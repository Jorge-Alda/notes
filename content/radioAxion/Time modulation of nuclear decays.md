---
title: Time modulation of nuclear decays
tags:
  - ALP
  - RadioAxion
  - Nuclear
---
Taylor expansion of the decay width [[Theta-dependence of nuclear decays]] [^1][^2]

$$\Gamma(\theta)\approx\Gamma(0)+\mathring{\Gamma}(0) \theta^2\,,\qquad \mathring{f}\equiv \frac{d f}{d(\theta^2)}$$


$\theta$ itself is time dependent
- [[Misalignment mechanism]]
- [[Stochastic dark matter]]

Our observable is given by [^2]

$$I(t) \equiv \frac{\Gamma(\theta(t)) - \langle\Gamma\rangle}{\langle\Gamma\rangle} = \frac{1}{2}\frac{\mathring{\Gamma}(0)}{\Gamma(0)}\theta_0^2 \cos(2m_at+\varphi) =3.4\times10^{-4} \cos(2m_at+\varphi) \left(\frac{\rho_\mathrm{DM}}{0.45 \mathrm{GeV}/\mathrm{cm}^3}\right) \left(\frac{10^{-16}\,\mathrm{eV}}{m_a}\right)^2\left(\frac{10^8\,\mathrm{GeV}}{f_a}\right)^2\left(\frac{\mathring{\Gamma}(0)}{\Gamma(0)}\right)$$

$\mathring{\Gamma}(0)/\Gamma(0)$ contains the nuclear physics input, and sets the overall sensitivity of the experiments:
- ${}^{241}\mathrm{Am}\to {}^{237}\mathrm{Np}^\star + \alpha + \gamma$: $\mathring{\Gamma}(0)/\Gamma(0)=-125$ [^1]
-  ${}^{40}\mathrm{K}\to{}^{40}\mathrm{Ar}^\star$: $\mathring{\Gamma}(0)/\Gamma(0)=18.8$ [^2]
-  ${}^{137}\mathrm{Cs}\to {}^{137}\mathrm{Ba}^{\star\star}$: $\mathring{\Gamma}(0)/\Gamma(0)=-2.13$ [^2]

## Nuclear decays revisited

If the decay rate does not depend on time, the number of radioactive nuclei in the source at time $t$ is $$N(t) = N_0 \exp(-\Gamma t)$$ and if we observe the source from time $t_0$ to time $t_0 + \Delta t$ with $\Delta t \ll 1/\Gamma$ (as is the case in the americium decays), the expected number of decays is $$\Delta N(t_0) = N(t_0) - N(t_0+\Delta t) = N_0 [\exp(-\Gamma t_0)-\exp(-\Gamma (t_0+\Delta t))]\approx N_0 \Gamma \Delta t \exp(-\Gamma t_0)$$ while the actual number of decays is a Poisson variable $\sim \mathrm{Poiss}(\Delta N)$.

Now, if $\Gamma$ itself depends on time due to the variation of $\theta$,
$$N(t) = N_0 \exp(-\Gamma(t)t) = N_0 \exp[-(\Gamma(0)+\mathring{\Gamma}(0)\theta^2(t))t]\approx N_0 \exp(-\Gamma(0)t)(1 - \mathring{\Gamma}(0)t\theta^2(t) )$$again we assume $\Delta t \ll 1/\Gamma(0)$. However, we do not make any assumptions regarding the relative scale between $\Delta t$ and $1/m_a$, so we can not expand the dependence of $\theta(t)$ $$\Delta N = N_0 \Gamma(0) \Delta t \exp(-\Gamma(0)t_0)\left[1 - \frac{\mathring{\Gamma}(0)}{\Gamma(0)}\left(\frac{t_0}{\Delta t}\theta^2(t_0) - \frac{t_0+\Delta t}{\Delta t}\theta^2(t_0+\Delta t) \right) \right]$$
In particular for the "deterministic" scenario $\theta(t) = \frac{\sqrt{2\rho_\mathrm{DM}}}{m_a f_a} \cos(m_a t + \varphi)$, $$\Delta N(t_0) = N_0 \Gamma(0) \Delta t \exp(-\Gamma(0)t_0)\left[1-\frac{\mathring{\Gamma}(0)}{\Gamma(0)}\frac{2\rho_\mathrm{DM}}{m_a^2 f_a^2}\left(\frac{t_0}{\Delta t}\cos^2(m_a t_0+\varphi) - \frac{t_0+\Delta t}{\Delta t}\cos^2(m_at_0+m_a\Delta t + \varphi) \right)\right]$$
Taking a time-average over a period long enough to smooth the axion oscillations but short enough that the number of radioactive nuclei has not changed significantly, $$\langle \Delta N(t_0)\rangle = N_0 \Gamma(0) \Delta t \exp(-\Gamma(0)t_0)\left[1+\frac{\mathring{\Gamma}(0)}{\Gamma(0)}\frac{\rho_\mathrm{DM}}{m_a^2 f_a^2}\right]$$  $$I(t_0) = \frac{\Delta N(t_0)-\langle\Delta N(t_0)\rangle}{\langle \Delta N(t_0)\rangle} =- \frac{\mathring{\Gamma}(0)}{\Gamma(0)}\frac{2\rho_\mathrm{DM}}{m_a^2 f_a^2}\left(\frac{1}{2}+\frac{t_0}{\Delta t}\cos^2(m_a t_0+\varphi) - \frac{t_0+\Delta t}{\Delta t}\cos^2(m_at_0+m_a\Delta t + \varphi) \right)$$
## Bibliography

[^1]: [[Alpha radioactivity deep-underground as a probe of axion dark matter (2404.18993v2)]]

[^2]:[[Weak nuclear decays deep-underground as a probe of axion dark matter (2412.20932v2)]]
