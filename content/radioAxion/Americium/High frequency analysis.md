
Goal: Analysis of frequencies between 1Hz and 500kHz, with resolution of 1Hz.

I have been re-checking my code, and there are a few aspects of the analysis for the data at high frequencies, and there are some issues that I do not know how to deal with.

First there is the issue of the mismatch between the two time informations. We have the Rb clock, that provides pulses every 1s, and the timestamps of the events, in "microseconds". But the separation between Rb pulses, according to the timestamps, fluctuates between 1000092 and 1000097 "microseconds". My naive solution was to rescale the timestamps within each 1s-period so that the separation between consecutive Rb pulses is indeed 1000000 microseconds. But this means that the timestamps are not evenly distributed, and therefore the Fourier analysis is not valid: either Lomb-Scargle or fitting must be used instead. And even if the Fourier analysis would be valid, the DFT frequencies would not be integer multiples of 1Hz, but of 1000000/1000009xHz

## Likelihood

Our data is structured as an sparse list: we have the timestamps corresponding to the event detections, while times without detections are not in the list. We will exploit this sparsity to improve the efficiency of the calculations.

$$\begin{align}N(t) =& N_0 \exp(-\Gamma t)\\ \Delta N =& N_0\exp(-\Gamma t) [1-\exp(-\Gamma \Delta t)]\approx N_0 \Gamma \Delta t \end{align}$$
Observed number of decays follows a Poisson distribution with $\lambda = N_0 \Gamma \Delta t$

- Null hypothesis $H_0$: $\lambda(t) = \lambda_0$
- Alternative hypothesis $H_1$: $\lambda(t) = \lambda_0(1+ A_\omega^2 \cos^2(\omega t + \varphi))$

The $H_1$ is a inhomogeneous Poisson process, while $H_0$ is obviously an homogeneous case.

We split our data in subintervals of $T_0=1\,\mathrm{s}$. The log-likelihood for each subinterval $j$ is
$$\begin{align}
\log \ell^{H_1}_j &= \sum_i \log \lambda(t_{i,j})-\int_{t_{0, j}}^{t_{0,j} + T_0} \lambda(t)\, dt \\
&= N_j \log \lambda_0-\lambda_0 T_0(1+A_\omega^2/2) + A_\omega^2 \sum_i \cos^2(\omega t_{i,j}+\varphi_j)
\end{align}$$

$$\log\ell^{H_1} = \sum_j \ell_j^{H_1} = N \log \lambda_0 - \lambda_0 T (1+A_\omega^2/2) + A_\omega^2 \sum_{i,j}\cos^2(\omega t_{i,j}+\varphi_j)$$

$$\begin{align}
\sum_{i} \cos^2(\omega t_{i,j} + \varphi_j) &= \sum_{i}[\cos(\omega t_{i,j})\cos\varphi_j - \sin(\omega t_{i,j})\sin\varphi_j]^2\\
&= \cos^2\varphi_j \sum_{i} \cos^2(\omega t_{i,j}) + \sin^2\varphi_j\sum_{i}\sin^2(\omega t_{i,j}) - 2 \sin\varphi_j \cos\varphi_j \sum_{i} \sin(\omega t_{ij})\cos(\omega t_{i,j})\\
&= \frac{1}{4}[1 + \cos(2\varphi_j)]\sum_{i}[1 +\cos(2\omega t_{i,j})] + \frac{1}{4}[1-\cos(2\varphi_j)] \sum_{i}[1-\cos(2\omega t_{i,j})]-\frac{1}{2}\sin(2\varphi_j)\sum_{i} \sin(2\omega t_{i,j})\\
&= \frac{N_j}{2}+\frac{1}{2}\cos(2\varphi_j)\sum_{i}\cos(2\omega t_{i,j})-\frac{1}{2}\sin(2\varphi_j)\sum_{i} \sin(2\omega t_{i,j})
\end{align}$$

$$\frac{\partial}{\partial\varphi_j} \sum_{i} \cos^2(\omega t_{i,j} + \varphi_j) = -\sin(2\varphi_j) \sum_{i} \cos(2\omega t_{i,j}) - \cos(2\varphi_j) \sum_{i} \sin(2\omega t_{i,j})=0$$
$$\tan(2\varphi_j) = - \frac{\sum_{i} \sin(2\omega t_{i,j})}{\sum_{i} \cos(2\omega t_{i,j})}\qquad \sin(2\varphi_j) = -\frac{\sum_{i} \sin(2\omega t_{i,j})}{\sqrt{\left[\sum_{i} \sin(2\omega t_{i,j})\right]^2 + \left[\sum_{i} \cos(2\omega t_{i,j})\right]^2}}\qquad \cos(2\varphi_j) = \frac{\sum_{i} \cos(2\omega t_{i,j})}{\sqrt{\left[\sum_{i} \sin(2\omega t_{i,j})\right]^2 + \left[\sum_{i} \cos(2\omega t_{i,j})\right]^2}} $$

$$\left.\sum_{i} \cos^2(\omega t_{i,j} + \varphi_j)\right|_{\varphi_j} = \frac{N_j}{2}+\frac{1}{2}\sqrt{\left[\sum_{i} \sin(2\omega t_{i,j})\right]^2 + \left[\sum_{i} \cos(2\omega t_{i,j})\right]^2}$$

$$\log\ell^{H_1}_j = N_j(\log \lambda_0 + A_\omega^2/2)-\lambda_0 T_0(1+A_\omega^2/2) + \frac{A_\omega^2}{2}\sqrt{\left[\sum_{i} \sin(2\omega t_{i,j})\right]^2 + \left[\sum_{i} \cos(2\omega t_{i,j})\right]^2}$$

$$\log\ell^{H_1} = N(\log \lambda_0 + A_\omega^2/2)-\lambda_0 T(1+A_\omega^2/2) + \frac{A_\omega^2}{2}\sum_j\sqrt{\left[\sum_{i} \sin(2\omega t_{i,j})\right]^2 + \left[\sum_{i} \cos(2\omega t_{i,j})\right]^2}$$

$$\log \ell^{H_0} = N \log\lambda_0 -\lambda_0 T$$
$$2\Delta \log \ell = A_\omega^2\left[N-\lambda_0 T + \sum_j\sqrt{\left[\sum_{i} \sin(2\omega t_{i,j})\right]^2 + \left[\sum_{i} \cos(2\omega t_{i,j})\right]^2}\right]$$
but the MLE estimator for $\lambda_0$ is $\hat{\lambda}_0 = N/T$, so
$$2\Delta \log\ell = A_\omega^2\sum_j\sqrt{\left[\sum_{i} \sin(2\omega t_{i,j})\right]^2 + \left[\sum_{i} \cos(2\omega t_{i,j})\right]^2}$$
According to Wilk's theorem, this is distributed as a $\chi^2$ with 1 degree of freedom, so for a 95% CL,
$$A_\omega^2 = \frac{\chi^2_1(0.95)}{\sum_j\sqrt{\left[\sum_{i} \sin(2\omega t_{i,j})\right]^2 + \left[\sum_{i} \cos(2\omega t_{i,j})\right]^2}} = \frac{3.841}{\sum_j\sqrt{\left[\sum_{i} \sin(2\omega t_{i,j})\right]^2 + \left[\sum_{i} \cos(2\omega t_{i,j})\right]^2}}$$


Testing for multiple frequencies: 
- Bonferroni: $\alpha_B = \alpha/{n_f}$. For $n_f=5\times10^{-5}$, we have to plug-in $\chi^2_1(1-10^{-7})=26.296$. Extremely conservative.
- FDR for "interesting" frequencies