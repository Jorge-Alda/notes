---
title: ALP Chiral Perturbation Theory
draft: false
tags:
  - ALP
  - ChiPT
---
 We begin with the parton-level Lagrangian (see [[Chiral Perturbation Theory]])
 
$$\mathcal{L}=-\frac{1}{4}G_{\mu\nu}^a G^{\mu\nu,a}+i\bar{q}\cancel D q-\bar{q} \boldsymbol{m_q} P_L q - \bar{q}\boldsymbol{m_q}^\dagger P_R q + \frac{\partial_\mu a}{f_a}\bar{q}\gamma^\mu(\boldsymbol{c_q^R}P_R + \boldsymbol{c_q^L}P_L)q + \frac{\alpha_s}{4\pi}\left(\frac{c_G}{f_a}a-\frac{\theta_0}{2}\right)G_{\mu\nu}\tilde{G}^{\mu\nu,a}+\frac{1}{2}\partial_\mu a \partial^\mu a - \frac{\mu_a^2}{2}a^2$$
We make the following identifications:
- $\boldsymbol{S} + i \boldsymbol{P} = \frac{\boldsymbol{\chi}}{2B_0} = \boldsymbol{m_q} = \mathrm{diag}(m_u e^{i\alpha_u}, m_d e^{i\alpha_d}, m_s e^{i\alpha_s})$
- $\boldsymbol{L}_\mu = \boldsymbol{c_q^L} \frac{\partial_\mu a}{f_a}$
- $\boldsymbol{R}_\mu = \boldsymbol{c_q^R} \frac{\partial_\mu a}{f_a}$
- $\theta = \theta_0 -2\frac{c_G}{f_a}a$

The low-energy Lagrangian becomes
$$\mathcal{L}=\frac{F_0^2}{2}\langle D_\mu \boldsymbol{U} D^\mu\boldsymbol{U}^\dagger\rangle + F_0^2 B_0\langle \boldsymbol{m_q} \boldsymbol{U}^\dagger + \boldsymbol{m_q}^\dagger\boldsymbol{U}\rangle -\frac{F_0^2 m_0^2}{12}\left[\theta_0-2\frac{c_G}{f_a}a-i\langle \log\boldsymbol{U} - \log\boldsymbol{U}^\dagger\rangle\right]^2 +\frac{1}{2}\partial_\mu a \partial^\mu a - \frac{\mu_a^2}{2}a^2$$ $$D_\mu\boldsymbol{U}=\partial_\mu\boldsymbol{U}-i\frac{\partial_\mu a}{f_a}(\boldsymbol{c_q^R}\boldsymbol{U}-\boldsymbol{U}\boldsymbol{c_q^L})$$

# Axion potential and neutron edm

$$V(a) = -F_0^2 [m_u \cos(\alpha_u-\varphi_u)+m_d \cos(\alpha_d-\varphi_d)+m_s \cos(\alpha_s-\varphi_s)]+\frac{m_0^2}{12}F_0^2\left[\theta_0-2\frac{c_G}{f_a}a + \varphi_u+\varphi_d+\varphi_s\right]^2+\frac{\mu_a^2}{2}a^2$$
The minimum of the ALP field is located at $$\langle a\rangle = \frac{c_G}{f_a}\frac{m_0^2 F_0^2}{3 m_a^2}(\theta_0 + \varphi_u + \varphi_d + \varphi_s)$$ where the "physical" (not really, we still must diagonalize the quadratic terms!!!) mass is $$m_a^2 = \mu_a^2 +\frac{2}{3} c_G^2\frac{F_0^2}{f_a^2}m_0^2$$
 By shifting the ALP field from its minimum $a\to a - \langle a \rangle$,
 
$$V =  -F_0^2 
 B_0 [m_u \cos(\alpha_u-\varphi_u)+m_d \cos(\alpha_d-\varphi_d)+m_s \cos(\alpha_s-\varphi_s)] +\frac{1}{2}m_a^2 a^2 +\frac{m_0^2}{12}F_0^2 \frac{\mu_a^2}{m_a^2}(\theta_0+\varphi_u + \varphi_d+\varphi_s)^2$$

$$B_0 m_u \sin(\alpha_u -\varphi_u) = B_0 m_d \sin(\alpha_d-\varphi_d) = B_0 m_s \sin(\alpha_s-\varphi_s)=\frac{m_0^2}{6}\frac{\mu_a^2}{m_a^2}(\theta_0+\varphi_u+\varphi_d+\varphi_s)
$$

Note that if $\mu_a = 0$ (aka QCD axion), then $\varphi_i = \alpha_i$ irrespective of the value of $\theta_0$, and in that case [[Chiral Perturbation Theory#^e54958]] gives $\tilde{m}=0$ and $d_n=0$, solving the strong CP problem.
  For $\mu_a \neq 0$ and $\bar\theta$ small
 $$\varphi_i \approx \alpha_i - \frac{m_i^{-1}}{\mathrm{tr}(|\boldsymbol{m_q}|^{-1})+\frac{6B_0}{m_0^2}\frac{m_a^2}{\mu_a^2}}\bar{\theta}$$
$$\tilde{m} = \frac{1}{\mathrm{tr}(|\boldsymbol{m_q}|^{-1})+\frac{6B_0}{m_0^2}\frac{m_a^2}{\mu_a^2}}$$

In the limit of heavy ALP $m_a^2 \approx \mu_a^2$ and the prediction for $d_n$ tends to the SM, and the strong CP problem persists. If $\mu_a^2 \ll m_a^2$,
$$\tilde{m}\approx \frac{m_0^2}{6B_0}\frac{\mu_a^2}{m_a^2} = \frac{\mu_a^2 f_a^2(m_u+m_d)}{4c_G^2 m_\pi^2 F_0^2}$$
In order to remain consistent with the neutron edm while having $|\bar{\theta}|\sim1$, $$\frac{\mu_a^2 f_a^2}{c_G^2}<1.4\times10^{-10}m_\pi^2 F_0^2$$ Axion Quality problem!!!

# Mixing of pseudoscalar fields at LO

According to Srednicki, eq.(94.18), the full pseudoscalar matrix with a non-trivial vev is
$$\boldsymbol{U} =\boldsymbol{u_0}\exp\left(\frac{i}{F_0}\boldsymbol{\lambda_a} \pi^a\right)\boldsymbol{u_0}\equiv\boldsymbol{u_0}\boldsymbol{\bar U}\boldsymbol{u_0} \qquad \boldsymbol{u_0}^2 = \boldsymbol{U_0}=\exp(i\boldsymbol{\varphi})$$

In the $U(1)_A$ piece of the Lagrangian, the vev just shifts $\theta \to \bar{\theta}$, and its effects are already accounted in the vev of the axion.
For the quark-mass piece, we observe that
$$\langle \boldsymbol{m_q}^\dagger \boldsymbol{u_0} \boldsymbol{\bar U}\boldsymbol{u_0}\rangle = \langle \boldsymbol{m_q}^\dagger \boldsymbol{U_0}\boldsymbol{\bar U}\rangle \approx \langle (|\boldsymbol{m_q}|-i\tilde{m}\bar{\theta})\boldsymbol{\bar U}\rangle$$
$$\langle \boldsymbol{m_q}^\dagger \boldsymbol{U} + \boldsymbol{U}^\dagger \boldsymbol{m_q}\rangle = \langle |\boldsymbol{m_q}|(\boldsymbol{\bar U} + \boldsymbol{\bar U}^\dagger)\rangle + i \tilde{m}\bar\theta \langle \boldsymbol{\bar U}^\dagger-\boldsymbol{\bar U}\rangle $$
where the first term is the usual of $\chi$PT without complex masses and/or $\theta$ angles, and the second will introduce vertices with an odd number of pNGBs, albeit very suppressed (it is proportional to $d_n$!)

The troubles come from the kinetic term. The covariant derivative is
$$D_\mu \boldsymbol{U} = \boldsymbol{u_0} \,\partial_\mu\boldsymbol{\bar U}\boldsymbol{u_0}-i\boldsymbol{R}_\mu \boldsymbol{u_0}\boldsymbol{\bar U}\boldsymbol{u_0} + i \boldsymbol{u_0}\boldsymbol{\bar U}\boldsymbol{u_0} \boldsymbol{L}_\mu = \boldsymbol{u_0} \left[\partial_\mu\boldsymbol{\bar U}-i\boldsymbol{\bar R}_\mu \boldsymbol{\bar U} + i\boldsymbol{\bar U} \boldsymbol{\bar L}_\mu \right]\boldsymbol{u_0} \equiv \boldsymbol{u_0} (\bar D_\mu \boldsymbol{\bar U})\boldsymbol{u_0}$$
$$\boldsymbol{\bar R}_\mu = \boldsymbol{u_0}^\dagger \boldsymbol{R}_\mu \boldsymbol{u_0}\qquad \boldsymbol{\bar L}_\mu = \boldsymbol{u_0} \boldsymbol{L}_\mu \boldsymbol{u_0}^\dagger$$
$$\langle D_\mu \boldsymbol{U}\,D^\mu \boldsymbol{U}^\dagger \rangle = \langle \bar D_\mu \boldsymbol{\bar U}\,\bar D^\mu \boldsymbol{\bar U}^\dagger \rangle$$

In the case of an ALP with off-diagonal quark couplings,
$$\boldsymbol{\bar A}_\mu = \boldsymbol{\bar L}_\mu - \boldsymbol{\bar R}_\mu = \frac{\partial_\mu a}{f_a}\begin{pmatrix}c_{uu}^A & 0 & 0 \\ 0 & c_{dd}^A & c_{ds}^A \cos\frac{\varphi_d-\varphi_s}{2}+ i c_{ds}^V\sin\frac{\varphi_d-\varphi_s}{2}\\ 0 & c_{sd}^A \cos\frac{\varphi_d-\varphi_s}{2}- i c_{sd}^V\sin\frac{\varphi_d-\varphi_s}{2} & c_{ss}^A \end{pmatrix} $$
Not only the axial and vectorial couplings mix, but this mixing angle is determined mostly by the phases of the quark masses, which are arbitrary(???). This will impact the mixing of the axion with the neutral kaons. $\bar{c}_{ds}^A = c_{ds}^A \cos\frac{\varphi_d-\varphi_s}{2}+ i c_{ds}^V\sin\frac{\varphi_d-\varphi_s}{2}$

We follow the steps of[^1], but introducing the derivative coupling to quarks in addition to the anomalous couplings to gluons[^2].

## Diagonalization of the kinetic term

We define the fields $$\begin{pmatrix}\eta\\ \eta'\end{pmatrix}=\begin{pmatrix}c_\eta & -s_\eta\\ s_\eta & c_\eta\end{pmatrix}\begin{pmatrix}\eta_8\\\eta_0\end{pmatrix} $$ which are orthogonal at LO. We will use as hadronic inputs $m_{\bar{K}}^2$, $\Delta^2 = m_{\bar{K}}^2 - m_{\bar{\pi}}^2$ and $\epsilon_I = B_0 (m_u-m_d) = m_{K^+}^2 - m_{K^0}^2-(m_{\pi^+}^2-m_{\pi^0}^2)$. At LO, the quark masses are $$|\boldsymbol{m_q}|=\frac{1}{2B_0}\begin{pmatrix}m_{\bar{K}}^2-\Delta^2 + \epsilon_I & 0 & 0\\ 0 & m_{\bar{K}}^2-\Delta^2 - \epsilon_I & 0\\ 0 & 0 & m_{\bar{K}}^2+\Delta^2\end{pmatrix}$$
With this, the masses of the eta mesons and their mixing angle are 
$$\begin{align}
m_\eta^2 &= m_{\bar{K}}^2 + \frac{1}{2}m_0^2 - \frac{1}{2}\sqrt{m_0^4 -\frac{4}{3}m_0^2 \Delta^2 + 4\Delta^4}\\ 
m_{\eta'}^2 &= m_{\bar{K}}^2 + \frac{1}{2}m_0^2 + \frac{1}{2}\sqrt{m_0^4 -\frac{4}{3}m_0^2 \Delta^2 + 4\Delta^4}\\
\cos(2\theta_\eta) &= 2 c_\eta^2-1 = \frac{\frac{2}{3}\Delta^2-m_0^2}{\sqrt{m_0^4 -\frac{4}{3} m_0^2 \Delta^2 + 4\Delta^4}}
\end{align}$$

The quadratic terms, written with the Lagrangian fields, are
$$\begin{align}
\mathcal{L}\supset&\frac{1}{2}\partial_\mu \pi^0 \partial^\mu \pi^0 + \frac{1}{2}\partial_\mu \eta \partial^\mu \eta + \frac{1}{2}\partial_\mu \eta' \partial^\mu \eta'+\partial_\mu K^0\partial^\mu \bar K^0+\frac{1}{2}\partial_\mu a \partial^\mu a-\frac{F_0}{f_a}\partial_\mu a\left[\langle\boldsymbol{\bar c_q^A}\boldsymbol{\lambda_{\pi^0}}\rangle \partial^\mu \pi^0 + \langle\boldsymbol{\bar c_q^A}\boldsymbol{\lambda_{\eta}}\rangle \partial^\mu \eta + \langle\boldsymbol{\bar c_q^A}\boldsymbol{\lambda_{\eta'}}\rangle \partial^\mu \eta' + \langle\boldsymbol{\bar c_q^A}\boldsymbol{\lambda_{K^0}}\rangle \partial^\mu K^0 + \langle\boldsymbol{\bar c_q^A}\boldsymbol{\lambda_{\bar K^0}}\rangle \partial^\mu \bar K^0\right]\\
&-\frac{1}{2}m_\pi^2 {\pi^0}^2 -\frac{1}{2}m_\eta^2 \eta^2 - \frac{1}{2}m_{\eta'}^2 {\eta'}^2-m_{K^0}^2 K^0 \bar K^0-\frac{1}{2}\left(\mu_a^2 +\frac{2}{3}c_G^2\frac{F_0^2}{f_a^2}m_0^2\right) a^2-\epsilon_I\frac{c_\eta-\sqrt{2}s_\eta}{\sqrt{3}} \pi^0 \eta -\epsilon_I \frac{s_\eta + \sqrt{2}c_\eta}{\sqrt{3}}\pi^0 \eta' + \sqrt{\frac{2}{3}}m_0^2 c_G \frac{F_0}{f_a} (c_\eta \eta' - s_\eta \eta) a
\end{align}$$

$$\begin{pmatrix}\pi^0_{(ph)}\\ \eta_{(ph)}\\ \eta'_{(ph)}\\ K^0_{(ph)} \\ \bar K^0_{(ph)}\\ a_{(ph)}\end{pmatrix} = \begin{pmatrix}1 & -\theta_{\pi^0\eta} & -\theta_{\pi^0 \eta'} & 0 & 0 & \epsilon_a \theta_{\pi^0 a}\\ \theta_{\pi^0\eta} & 1 & 0 & 0 & 0 & \epsilon_a \theta_{\eta a}\\ \theta_{\pi^0\eta'} & 0 & 1 & 0 & 0 & \epsilon_a \theta_{\eta' a}\\ 0 & 0 & 0 & 1 & 0 & \epsilon_a\theta_{K^0 a}\\ 0 & 0 & 0 & 0 & 1 & \epsilon_a \theta_{\bar K^0 a}\\ \epsilon_a \theta_{a \pi^0} & \epsilon_a \theta_{a\eta} & \epsilon_a \theta_{a\eta'} & \epsilon_a \theta_{a K^0} & \epsilon_a \theta_{a \bar K^0} & 1 + \epsilon_a^2 \theta_{aa}\end{pmatrix} \begin{pmatrix}\pi^0\\ \eta\\ \eta'\\ K^0 \\ \bar K^0 \\ a\end{pmatrix} $$

$$\begin{align}
\theta_{\pi^0\eta} &= -\frac{\epsilon_I}{\sqrt{3}}\frac{c_\eta - \sqrt{2}s_\eta}{m_\eta^2 - m_{\pi^0}^2}\\
\theta_{\pi^0\eta'} &= -\frac{\epsilon_I}{\sqrt{3}}\frac{\sqrt{2}c_\eta+ s_\eta}{m_{\eta'}^2 - m_{\pi^0}^2}\\
 \theta_{a\pi^0} + \theta_{\pi^0 a}-\theta_{\pi^0\eta}\theta_{\eta a} - \theta_{\pi^0\eta'} \theta_{\eta' a} &= -\langle \boldsymbol{\bar c_q^A}\boldsymbol{\lambda_{\pi^0}}\rangle\\
\theta_{a\eta} + \theta_{\eta a}+\theta_{\pi^0\eta}\theta_{\pi^0 a}&= -\langle \boldsymbol{\bar c_q^A}\boldsymbol{\lambda_{\eta}}\rangle  \\
 \theta_{a\eta'} + \theta_{\eta' a}-\theta_{\pi^0\eta'}\theta_{\pi^0 a}&= -\langle \boldsymbol{\bar c_q^A}\boldsymbol{\lambda_{\eta'}}\rangle\\
\theta_{a K^0} + \theta_{\bar K^0 a} &= -\langle \boldsymbol{\bar c_q^A}\boldsymbol{\lambda_{K^0}}\rangle \\
\theta_{a \bar K^0} + \theta_{K^0 a}&= -\langle \boldsymbol{\bar c_q^A}\boldsymbol{\lambda_{\bar K^0}}\rangle\\
2 \theta_{aa} + \theta_{\pi^0 a}^2+ \theta_{\eta a}^2 + \theta_{\eta' a}^2 + 2 \theta_{K^0a}\theta_{\bar K^0a} &= 0\\
 m_a^2 \theta_{a\pi^0} + m_{\pi^0}^2 \theta_{\pi^0 a} - m_\eta^2 \theta_{\pi^0\eta} \theta_{\eta a} - m_{\eta'}^2 \theta_{\pi^0 \eta'} \theta_{\eta' a} &= 0\\
 m_a^2 \theta_{a\eta} + m_\eta^2 \theta_{\eta a} + m_{\pi^0}^2 \theta_{\pi^0 \eta}\theta_{\pi^0 a} &= -\sqrt{\frac{2}{3}}m_0^2 s_\eta c_G\\
m_a^2 \theta_{a\eta'} + m_{\eta'}^2 \theta_{\eta' a} + m_{\pi^0}^2 \theta_{\pi^0 \eta'}\theta_{\pi^0 a} &= \sqrt{\frac{2}{3}}m_0^2 c_\eta c_G \\
m_a^2 \theta_{a K^0} + m_{K^0}^2 \theta_{\bar K ^0 a} = 0\\
m_a^2 \theta_{a \bar K^0} + m_{K^0}^2 \theta_{K ^0 a} = 0\\
m_a^2 + \frac{F_0^2}{f_a^2}(m_{\pi^0}^2 \theta_{\pi^0 a}^2 + m_{\eta}^2 \theta_{\eta^0 a}^2 + m_{\eta'}^2 \theta_{\eta' a}^2 +2m_{K^0}^2 \theta_{K^0 a}\theta_{\bar{K}^0 a} +2 m_a^2\theta_{aa}) &= \mu_a^2 + \frac{2}{3}c_G^2\frac{F_0^2}{f_a^2}m_0^2
\end{align}$$

$$ \begin{pmatrix}
m_{\pi^0}^2 - m_a^2 & -(m_\eta^2 - m_a^2)\theta_{\pi^0 \eta}  & -(m_{\eta'}^2 - m_a^2)\theta_{\pi^0 \eta'}\\(m_{\pi^0}^2 - m_a^2)\theta_{\pi^0 \eta} & m_\eta^2 - m_a^2 & 0 \\(m_{\pi^0}^2 - m_{a}^2)\theta_{\pi^0 \eta'} & 0 & m_{\eta'}^2-m_a^2
\end{pmatrix}\begin{pmatrix}
\theta_{\pi^0 a} \\ \theta_{\eta a} \\ \theta_{\eta' a}
\end{pmatrix} = \begin{pmatrix}
m_a^2 \langle\boldsymbol{\bar c_q^A}\boldsymbol{\lambda_{\pi^0}}\rangle \\ m_a^2 \langle\boldsymbol{\bar c_q^A}\boldsymbol{\lambda_{\eta}}\rangle -\sqrt{\frac{2}{3}}m_0^2 s_\eta c_G \\ m_a^2 \langle\boldsymbol{\bar c_q^A}\boldsymbol{\lambda_{\eta'}}\rangle +\sqrt{\frac{2}{3}}m_0^2 c_\eta c_G
\end{pmatrix}$$

$$ \begin{pmatrix}
\theta_{\pi^0 a} \\ \theta_{\eta a} \\ \theta_{\eta' a}
\end{pmatrix}\approx\begin{pmatrix}
\frac{1}{m_{\pi^0}^2-m_a^2} & \frac{1}{m_{\pi^0}^2-m_a^2}\theta_{\pi^0 \eta}  & \frac{1}{m_{\pi^0}^2-m_a^2}\theta_{\pi^0 \eta'}\\
 - \frac{1}{m_{\eta}^2-m_a^2}\theta_{\pi^0 \eta} & \frac{1}{m_\eta^2-m_a^2} & 0\\ - \frac{1}{m_{\eta'}^2-m_a^2}\theta_{\pi^0 \eta'} & 0 & \frac{1}{m_{\eta'}^2-m_a^2}
\end{pmatrix}\begin{pmatrix}
m_a^2 \langle\boldsymbol{\bar c_q^A}\boldsymbol{\lambda_{\pi^0}}\rangle \\ m_a^2 \langle\boldsymbol{\bar c_q^A}\boldsymbol{\lambda_{\eta}}\rangle -\sqrt{\frac{2}{3}}m_0^2 s_\eta c_G \\ m_a^2 \langle\boldsymbol{\bar c_q^A}\boldsymbol{\lambda_{\eta'}}\rangle +\sqrt{\frac{2}{3}}m_0^2 c_\eta c_G
\end{pmatrix}$$

$$\theta_{K^0 a} = \frac{m_a^2}{m_{K^0}^2-m_a^2}\langle \boldsymbol{\bar c_q^A}\boldsymbol{\lambda_{\bar K^0}}\rangle\qquad \theta_{\bar K^0 a} = \frac{m_a^2}{m_{K^0}^2-m_a^2}\langle \boldsymbol{\bar c_q^A}\boldsymbol{\lambda_{ K^0}}\rangle$$

QCD axion, i.e. $c_u =c_d =c_s = 0$, $\mu_a^2=0$, $c_G=-1/2$:
$$\begin{align}
\theta_{\eta a} &= \frac{m_0^2}{\sqrt{6}m_\eta^2}s_\eta \\
\theta_{\eta' a} &=- \frac{m_0^2}{\sqrt{6}m_{\eta'}^2}c_\eta \\
m_a^2 &= \frac{m_0^2}{6}\frac{F_0^2}{f_a^2}\left(1 - \frac{m_0^2 s_\eta^2}{m_\eta^2} - \frac{m_0^2 c_\eta^2}{m_{\eta'}^2}\right)
\end{align}$$ 

Agreeing with 2211.02867, and consequently reproducing the well-known QCD axion mass when plugging the correct hadronic inputs (see discussion there...)

## v2

### Set-up and goals
- Completely generic axion(LP)
	- Anomalous coupling to gluons
	- Derivative coupling to light quarks
		- Off-diagonal couplings to $d-s$ quarks, either generated at loop order or via exotic UV models
	- Explicit mass term $\mu_a$
- Complex quark masses
- Non-zero $\theta$ term
- We will not perform any chiral rotation, neither to "eliminate" the anomalous gluon coupling nor to rotate away the phases of the quarks/$\theta$
- Instead, we will perform the full matching, including the $U(1)_A$ anomaly via Witten-Veneziano, which incorporates both the axion and $\theta$.
- The presence of a non-zero $\theta$ and/or complex quark masses requires a vev for $U$, $$\langle\boldsymbol{U}\rangle = \boldsymbol{u_0}^2$$ $$\boldsymbol{U} = \boldsymbol{u_0} \boldsymbol{\bar U}\boldsymbol{u_0}$$ where $\boldsymbol{\bar U}$ is the usual exponential of the pseudoscalar mesons
- Since the ALP can potentially mix with kaons, let us assume a more generic structure for the $d-s$ block of the vev of $U$, $$\boldsymbol{u_0} = \begin{pmatrix}\exp(i \varphi_{uu}) & 0 & 0\\ 0 & c_{u_0} \exp(i\varphi_{dd}) & -s_{u_0}\exp[i(\varphi_{dd} + \varphi_{ss}-\Delta_{sd})/2] \\ 0 & s_{u_0}\exp[i(\varphi_{dd} + \varphi_{ss}+\Delta_{sd})/2] & c_{u_0} \exp(i\varphi_{ss}) \end{pmatrix}$$
- We want to calculate
	- Mixing of the axion to pseudoscalars
	- Mass of the axion (QCD) or corrections (ALP)
	- Neutron edm
	- Quartic interactions
	- Decay to photons via WZW

### $U(1)_A$ anomaly
$$\langle \log u_0\rangle = \frac{1}{2} \log(\det u_0) = i(\varphi_{uu} + \varphi_{dd} + \varphi_{ss})/2$$

$$\langle \log U \rangle = 2\langle \log u_0 \rangle + \langle \log \bar U\rangle =i\left( \varphi_{uu} + \varphi_{dd} + \varphi_{ss} + \frac{\sqrt{6}}{2F_0}\eta_0\right)$$

$$\begin{align}
\mathcal{L}_{U(1)_A} =& -\frac{F_0^2 m_0^2}{12}\left[\theta_0 -\frac{2 c_G}{f_a}a+\frac{\sqrt{6}}{F_0}\eta_0 + 2\varphi_{uu}+2\varphi_{dd} + 2\varphi_{ss}\right]^2\\
&\supset \frac{c_G F_0^2 m_0^2}{3 f_a}(\theta_0 + 2\varphi_{uu}+2\varphi_{dd} + 2\varphi_{ss}) a\\
&-\frac{F_0 m_0^2}{\sqrt{6}}(\theta_0 + 2\varphi_{uu}+2\varphi_{dd} + 2\varphi_{ss}) \eta_0\\
&-\frac{1}{2}m_0^2\eta_0^2-\frac{1}{2}\frac{2 c_G^2 F_0^2 m_0^2}{3f_a^2}a^2\\
&+ \sqrt{\frac{2}{3}}\frac{c_G F_0 m_0^2}{f_a} a \eta_0
\end{align}$$

### $\chi$ mass term

We will use as hadronic inputs $m_{\bar{K}}^2$, $\Delta^2 = m_{\bar{K}}^2 - m_{\bar{\pi}}^2$ and $\epsilon_I = B_0 (m_u-m_d) = m_{K^+}^2 - m_{K^0}^2-(m_{\pi^+}^2-m_{\pi^0}^2)$. At LO, the quark masses are $$|\boldsymbol{m_q}|=\frac{1}{2B_0}\begin{pmatrix}m_{\bar{K}}^2-\Delta^2 + \epsilon_I & 0 & 0\\ 0 & m_{\bar{K}}^2-\Delta^2 - \epsilon_I & 0\\ 0 & 0 & m_{\bar{K}}^2+\Delta^2\end{pmatrix}$$
$$\langle \boldsymbol{m_q}^\dagger \boldsymbol{U} \rangle = \langle\boldsymbol{m_q}^\dagger \boldsymbol{u_0}\boldsymbol{\bar U}\boldsymbol{u_0} \rangle = \langle\boldsymbol{u_0}\boldsymbol{m_q}^\dagger \boldsymbol{u_0}\boldsymbol{\bar U} \rangle \equiv \langle \boldsymbol{\bar m_q}^\dagger \boldsymbol{\bar U} \rangle$$

$$\boldsymbol{\bar m_q} = \boldsymbol{u_0}^\dagger \boldsymbol{m_q}\boldsymbol{u_0}^\dagger = \begin{pmatrix}m_u e^{i(\alpha_u - 2\varphi_{uu})} &0 &0
\\ 0 & m_d e^{i(\alpha_d - 2\varphi_{dd})} c_{u_0}^2 - m_s e^{i(\alpha_s - \varphi_{dd}-\varphi_{ss})} s_{u_0}^2 & (m_d e^{i(\alpha_d -\varphi_{dd})} + m_s e^{i(\alpha_s - \varphi_{ss})}) e^{-i(\varphi_{dd} + \varphi_{ss} +\Delta_{sd})/2} s_{u_0} c_{u_0} \\
0 & -(m_d e^{i(\alpha_d - \varphi_{dd})} + m_s e^{i(\alpha_s -\varphi_{ss})}) e^{-i(\varphi_{dd} + \varphi_{ss} -\Delta_{sd})/2}s_{u_0}c_{u_0} & m_s e^{i(\alpha_s -2\varphi_{ss})} c_{u_0}^2 - m_d e^{i(\alpha_d - \varphi_{dd}-\varphi_{ss})}s_{u_0}^2
\end{pmatrix}$$

$$\begin{align}
\mathcal{L}_\chi &= F_0^2 B_0 \langle \boldsymbol{m_q}^\dagger \boldsymbol{U} + \boldsymbol{m_q} \boldsymbol{U}^\dagger \rangle= F_0^2 B_0 \langle \boldsymbol{\bar m_q}^\dagger \boldsymbol{\bar U} + \boldsymbol{\bar m_q} \boldsymbol{\bar U}^\dagger \rangle \\
&\supset -i F_0 B_0 \langle(\boldsymbol{\bar m_q}-\boldsymbol{\bar m_q}^\dagger)\boldsymbol{\Phi} \rangle -\frac{B_0}{2}\langle (\boldsymbol{\bar m_q}+\boldsymbol{\bar m_q}^\dagger)\boldsymbol{\Phi}^2 \rangle\\
&= \frac{F_0}{2}\left[\sin(\alpha_u - 2\varphi_{uu})(m_{\bar K}^2 - \Delta^2 + \epsilon_I) - c_{u_0}^2\sin(\alpha_d - 2\varphi_{dd}) (m_{\bar K}^2 -\Delta^2 -\epsilon_I) + s_{u_0}^2\sin(\alpha_s - \varphi_{dd}-\varphi_{ss})(m_{\bar K}^2 + \Delta^2) \right]\pi^0\\
&+ \frac{F_0}{2\sqrt{3}} \left[\sin(\alpha_u - 2\varphi_{uu})(m_{\bar K}^2 -\Delta^2 + \epsilon_I) + c_{u_0}^2 \sin(\alpha_d - 2\varphi_{dd})(m_{\bar K}^2-\Delta^2-\epsilon_I) -2c_{u_0}^2\sin(\alpha_s - 2\varphi_{ss})(m_{\bar K}^2 + \Delta^2)+2s_{u_0}^2 \sin(\alpha_d-\varphi_{dd}-\varphi_{ss})(m_{\bar K}^2-\Delta^2-\epsilon_I) - s_{u_0}^2 \sin(\alpha_s-\varphi_{dd}-\varphi_{ss})(m_{\bar K}^2 + \Delta^2)\right]\eta_8 \\
&+\frac{F_0}{\sqrt{6}}\left[\sin(\alpha_u - 2\varphi_{uu})(m_{\bar K}^2 -\Delta^2 + \epsilon_I) + c_{u_0}^2 \sin(\alpha_d - 2\varphi_{dd})(m_{\bar K}^2-\Delta^2-\epsilon_I) +c_{u_0}^2\sin(\alpha_s - 2\varphi_{ss})(m_{\bar K}^2 + \Delta^2)-s_{u_0}^2 \sin(\alpha_d-\varphi_{dd}-\varphi_{ss})(m_{\bar K}^2-\Delta^2-\epsilon_I) - s_{u_0}^2 \sin(\alpha_s-\varphi_{dd}-\varphi_{ss})(m_{\bar K}^2 + \Delta^2)\right]\eta_0\\
&+i \frac{F_0}{\sqrt{2}}s_{u_0} c_{u_0}\left[\cos(\alpha_d - 3 \varphi_{dd}/2-\varphi_{ss}/2)(m_{\bar K}^2-\Delta^2-\epsilon_I) + \cos(\alpha_s - \varphi_{dd}/2 -3\varphi_{ss}/2)(m_{\bar K}^2 +\Delta^2)\right] (e^{i \Delta_{sd}/2} K^0 - e^{-i \Delta_{sd}/2}\bar K^0)\\
&-\frac{1}{4}\left[\cos(\alpha_u -2\varphi_{uu})(m_{\bar K}^2 -\Delta^2+\epsilon_I)+c_{u_0}^2\cos(\alpha_d-2\varphi_{dd})(m_{\bar K}^2-\Delta^2-\epsilon_I)-s_{u_0}^2\cos(\alpha_s-\varphi_{dd}-\varphi_{ss})(m_{\bar K}^2 + \Delta^2)\right](\pi^0 \pi^0 + 2 \pi^+\pi^-)\\
&-\frac{1}{12}\left[\cos(\alpha_u-2\varphi_{uu})(m_{\bar K}^2 -\Delta^2 +\epsilon_I)+c_{u_0}^2 \cos(\alpha_d-2\varphi_{dd}) (m_{\bar K}^2-\Delta^2-\epsilon_I)+4c_{u_0}^2 \cos(\alpha_s-2\varphi_{ss})(m_{\bar K}^ 2+\Delta^2)-4s_{u_0}^2 \cos(\alpha_d-\varphi_{dd}-\varphi_{ss})(m_{\bar K}^2-\Delta^2-\epsilon_I)-s_{u_0}^2\cos(\alpha_s - \varphi_{dd}-\varphi_{ss})(m_{\bar K}^2+\Delta^2)\right]\eta_8^2\\
&-\frac{1}{6}\left[\cos(\alpha_u-2\varphi_{uu})(m_{\bar K}^2 -\Delta^2 +\epsilon_I)+c_{u_0}^2 \cos(\alpha_d-2\varphi_{dd}) (m_{\bar K}^2-\Delta^2-\epsilon_I)+c_{u_0}^2 \cos(\alpha_s-2\varphi_{ss})(m_{\bar K}^ 2+\Delta^2)-s_{u_0}^2 \cos(\alpha_d-\varphi_{dd}-\varphi_{ss})(m_{\bar K}^2-\Delta^2-\epsilon_I)-s_{u_0}^2\cos(\alpha_s - \varphi_{dd}-\varphi_{ss})(m_{\bar K}^2+\Delta^2)\right]\eta_0^2\\
&-\frac{1}{2}\left[c_{u_0}^2 \cos(\alpha_d-2\varphi_{dd})(m_{\bar K}^2 -\Delta^2 -\epsilon_I)+c_{u_0}^2\cos(\alpha_s-2\varphi_{ss})(m_{\bar K}^2+\Delta^2)-s_{u_0}^2 \cos(\alpha_d-\varphi_{dd}-\varphi_{ss})(m_{\bar K}^2 -\Delta^2 -\epsilon_I)-s_{u_0}^2\cos(\alpha_s-\varphi_{dd}-\varphi_{ss})(m_{\bar K}^2+\Delta^2)\right]K^0 \bar K^0\\
&-\frac{1}{2}\left[\cos(\alpha_u-2\varphi_{uu})(m_{\bar K}^2-\Delta^2+\epsilon_I)+c_{u_0}^2\cos(\alpha_s-2\varphi_{ss})(m_{\bar K}^2+\Delta^2)-s_{u_0}^2\cos(\alpha_d-\varphi_{dd}-\varphi_{ss})(m_{\bar K}^2-\Delta^2-\epsilon_I)\right]K^+ K^-\\
&-\frac{1}{2\sqrt{3}}\left[\cos(\alpha_u-2\varphi_{uu})(m_{\bar K}^2-\Delta^2+\epsilon_I)-c_{u_0}^2\cos(\alpha_d-2\varphi_{dd})(m_{\bar K}^2-\Delta^2-\epsilon_I)+s_{u_0}^2\cos(\alpha_s-\varphi_{dd}-\varphi_{ss})(m_{\bar K}^2+\Delta^2)\right](\pi^0\eta_8+\sqrt{2}\pi^0\eta_0)\\
&-\frac{i}{2\sqrt{2}}s_{u_0}c_{u_0}\left[\sin(\alpha_d-3\varphi_{dd}/2-\varphi_{ss}/2)(m_{\bar K}^2-\Delta^2-\epsilon_I)+\sin(\alpha_s-\varphi_{dd}-3\varphi_{ss}/2)(m_{\bar K}^2+\Delta^2)\right]\left(e^{i\Delta_{sd}/2}\pi^0 K^0-e^{-i\Delta_{sd}/2}\pi^0\bar K^0\right)\\
&-\frac{1}{3\sqrt{2}}\left[\cos(\alpha_u-2\varphi_{uu})(m_{\bar K}^2-\Delta^2+\epsilon_I)+c_{u_0}^2\cos(\alpha_d-2\varphi_{dd})(m_{\bar K}^2-\Delta^2-\epsilon_I)-2c_{u_0}^2\cos(\alpha_s-2\varphi_{ss})(m_{\bar K}^2+\Delta^2)+2s_{u_0}^2\cos(\alpha_d-\varphi_{dd}-\varphi_{ss})(m_{\bar K}^2-\Delta^2-\epsilon_I)-s_{u_0}^2\cos(\alpha_s-\varphi_{dd}-\varphi_{ss})(m_{\bar K}^2+\Delta^2)\right]\eta_0\eta_8\\
&-\frac{i}{2\sqrt{6}}s_{u_0}c_{u_0}\left[\sin(\alpha_d-3\varphi_{dd}/2-\varphi_{ss}/2)(m_{\bar K}^2-\Delta^2-\epsilon_I)+\sin(\alpha_s-\varphi_{dd}/2-3\varphi_{ss}/2)(m_{\bar K}^2+\Delta^2)\right](e^{i\Delta_{sd}/2}K^0-e^{-i\Delta_{sd}/2}\bar K^0)(\eta_8-2\sqrt{2}\eta_0)\\
&+\frac{i}{2}s_{u_0}c_{u_0}\left[\sin(\alpha_d-3\varphi_{dd}/2-\varphi_{ss}/2)(m_{\bar K}^2-\Delta^2-\epsilon_I)+\sin(\alpha_s-\varphi_{dd}/2-3\varphi_{ss}/2)(m_{\bar K}^2+\Delta^2)\right](e^{i\Delta_{sd}/2}K^+ \pi^- - e^{-i\Delta_{sd}/2}\pi^+ K^-)
\end{align}$$

### Kinetic term

$$\begin{align}
D_\mu \boldsymbol{U} =& \partial_\mu \boldsymbol{U} - i\frac{\partial_\mu a}{f_a}(\boldsymbol{c_q^R} \boldsymbol{U}-\boldsymbol{U}\boldsymbol{c_q^L})\\
=&\boldsymbol{u_0}(\partial_\mu \boldsymbol{\bar U})\boldsymbol{u_0}-i\frac{\partial_\mu a}{f_a}(\boldsymbol{c_q^R}\boldsymbol{u_0}\boldsymbol{\bar U}\boldsymbol{u_0}-\boldsymbol{u_0}\boldsymbol{\bar U}\boldsymbol{u_0}\boldsymbol{c_q^L})\\
=& \boldsymbol{u_0}\left[\partial_\mu \boldsymbol{\bar U} - i\frac{\partial_\mu a}{f_a}(\boldsymbol{\bar c_q^R} \boldsymbol{\bar U}-\boldsymbol{\bar U}\boldsymbol{\bar c_q^L})\right]\boldsymbol{u_0} \\
\equiv& \boldsymbol{u_0} (\bar D_\mu \boldsymbol{\bar U})\boldsymbol{u_0}\\
\supset& i \boldsymbol{u_0}\left[\frac{1}{F_0}\partial_\mu \boldsymbol{\Phi}+\frac{\partial_\mu a}{f_a}\boldsymbol{\bar c_q^A}\right]\boldsymbol{u_0}
\end{align}$$

$$\boldsymbol{\bar c_q^R}=\boldsymbol{u_0}^\dagger \boldsymbol{c_q^R}\boldsymbol{u_0}\,,\qquad \boldsymbol{\bar c_q^L}=\boldsymbol{u_0}\boldsymbol{c_q^L}\boldsymbol{u_0}^\dagger$$

$$\boldsymbol{\bar c_q^A} = \boldsymbol{\bar c_q^L}-\boldsymbol{\bar c_q^R} = \boldsymbol{u_0}\boldsymbol{c_q^L}\boldsymbol{u_0}^\dagger - \boldsymbol{u_0}^\dagger \boldsymbol{c_q^R}\boldsymbol{u_0}$$

$$\begin{align}
\bar c^A_{uu} &= c^A_{uu}\\
\bar c^A_{dd} &= c_{u_0}^2 c_{dd}^A + s_{u_0}^2 c_{ss}^A -  s_{u_0}c_{u_0}\left[i\sin(\varphi_{dd}/2-\varphi_{ss}/2)(e^{i\Delta_{sd}/2}c_{ds}^A - e^{-i\Delta_{sd}/2}c_{sd}^A)+\cos(\varphi_{dd}/2-\varphi_{ss}/2)(e^{i\Delta_{sd}/2}c_{ds}^V + e^{-i\Delta_{sd}/2}c_{sd}^V)\right]\\
\bar c_{ss}^A &= c_{u_0}^2 c_{ss}^A + s_{u_0}^2 c_{dd}^A + s_{u_0}c_{u_0}\left[i\sin(\varphi_{dd}/2-\varphi_{ss}/2)(e^{i\Delta_{sd}/2}c_{ds}^A - e^{-i\Delta_{sd}/2}c_{sd}^A)+\cos(\varphi_{dd}/2-\varphi_{ss}/2)(e^{i\Delta_{sd}/2}c_{ds}^V + e^{-i\Delta_{sd}/2}c_{sd}^V)\right]\\
\bar c_{ds}^A &=  [c_{u_0}^2\cos(\varphi_{dd}-\varphi_{ss}) -s_{u_0}^2 e^{-i\Delta_{sd}}]c_{ds}^A + i c_{u_0}^2 \sin(\varphi_{dd}-\varphi_{ss})c_{ds}^V+s_{u_0}c_{u_0}e^{-i\Delta_{sd}/2}\left[i\sin(\varphi_{dd}-\varphi_{ss})(c_{dd}^A-c_{ss}^A)+\cos(\varphi_{dd}-\varphi_{ss})(c_{dd}^V-c_{ss}^V)\right]\\
\bar c_{sd}^A &=  [c_{u_0}^2\cos(\varphi_{dd}-\varphi_{ss}) -s_{u_0}^2 e^{i\Delta_{sd}}]c_{sd}^A - i c_{u_0}^2 \sin(\varphi_{dd}-\varphi_{ss})c_{sd}^V+s_{u_0}c_{u_0}e^{i\Delta_{sd}/2}\left[-i\sin(\varphi_{dd}-\varphi_{ss})(c_{dd}^A-c_{ss}^A)+\cos(\varphi_{dd}-\varphi_{ss})(c_{dd}^V-c_{ss}^V)\right]
\end{align}$$

$$\begin{align}
\mathcal{L}_K =& \frac{F_0^2}{2}\langle D_\mu \boldsymbol{U} D^\mu \boldsymbol{U}^\dagger\rangle = \frac{F_0^2}{2}\langle \bar D_\mu \boldsymbol{\bar U} \bar D^\mu \boldsymbol{\bar U}^\dagger\rangle \\
\supset&\frac{1}{2} \left\langle \left(\partial_\mu\boldsymbol{\Phi} + \frac{F_0}{f_a}\partial_\mu a \,\boldsymbol{\bar c_q^A}\right)^2 \right\rangle = \frac{1}{2}\langle \partial_\mu \boldsymbol{\Phi}\partial^\mu \boldsymbol{\Phi}\rangle + \frac{F_0}{f_a}\partial_\mu a\langle\boldsymbol{\bar c_q^A} \partial^\mu\boldsymbol{\Phi}\rangle + \frac{F_0^2}{2f_a^2}\partial_\mu a\partial^\mu a \langle(\boldsymbol{\bar c_q^A})^2\rangle\\
=& \frac{1}{2}\partial_\mu \pi^0 \partial^\mu \pi^0 + \partial_\mu \pi^+\partial^\mu \pi^- + \frac{1}{2}\partial_\mu \eta_8 \partial^\mu \eta_8 +\frac{1}{2}\partial_\mu \eta_0 \partial^\mu \eta^0 + \partial_\mu K^0 \partial^\mu \bar K^0 + \partial_\mu K^+ \partial^\mu K^- \\
&+\frac{F_0}{2f_a}(\bar c_{uu}^A -\bar c_{dd}^A)\partial_\mu a \partial^\mu \pi^0\\
&+ \frac{F_0}{2\sqrt{3}f_a}(\bar{c}_{uu}^A +\bar c_{dd}^A -2 \bar c_{ss}^A) \partial_\mu a \partial^\mu \eta_8\\
&+ \frac{F_0}{\sqrt{6}f_a}(\bar c_{uu}^A + \bar c_{dd}^A +\bar c_{ss}^A)\partial_\mu a \partial^\mu \eta_0 \\
&+ \frac{F_0}{\sqrt{2}f_a}\bar c_{sd}^A \partial_\mu a \partial^\mu K^0 + \frac{F_0}{\sqrt{2}f_a}\bar c_{ds}^A \partial_\mu a \partial^\mu \bar K^0\\
&+ \frac{F_0^2}{4f_a^2}[(\bar c_{uu}^A)^2 + (\bar c_{dd}^A)^2 + (\bar c_{ss}^A)^2 + 2 \bar c_{ds}^A \bar c_{sd}^A]\partial_\mu a \partial^\mu a
\end{align}$$

### Total Lagrangian

$$\mathcal{L}_\mathrm{tot} = \frac{1}{2}\partial_\mu a \partial^\mu a -\frac{1}{2}\mu_a^2 a^2 + \mathcal{L}_K + \mathcal{L}_\chi + \mathcal{L}_{U(1)_A}$$

$$\begin{pmatrix}\pi^0_{(ph)}\\ \eta_{(ph)}\\ \eta'_{(ph)}\\ K^0_{(ph)} \\ \bar K^0_{(ph)}\\ a_{(ph)}\end{pmatrix} = \begin{pmatrix}1 & -\theta_{\pi^0\eta} & -\theta_{\pi^0 \eta'} & 0 & 0 & \epsilon_a \theta_{\pi^0 a}\\ \theta_{\pi^0\eta} & 1 & 0 & 0 & 0 & \epsilon_a \theta_{\eta a}\\ \theta_{\pi^0\eta'} & 0 & 1 & 0 & 0 & \epsilon_a \theta_{\eta' a}\\ 0 & 0 & 0 & 1 & 0 & \epsilon_a\theta_{K^0 a}\\ 0 & 0 & 0 & 0 & 1 & \epsilon_a \theta_{\bar K^0 a}\\ \epsilon_a \theta_{a \pi^0} & \epsilon_a \theta_{a\eta} & \epsilon_a \theta_{a\eta'} & \epsilon_a \theta_{a K^0} & \epsilon_a \theta_{a \bar K^0} & 1 + \epsilon_a^2 \theta_{aa}\end{pmatrix} \begin{pmatrix}\pi^0\\ c_\eta \eta_8 - s_\eta \eta_0\\ s_\eta \eta_8 + c_\eta \eta_0\\ K^0 \\ \bar K^0 \\ a+\langle a \rangle\end{pmatrix} $$


$$\begin{align}
\theta_{\pi^0 a} + \theta_{a \pi^0} + \theta_{\pi^0\eta}\theta_{\eta a} + \theta_{\pi^0 \eta'}\theta_{\eta' a} &= \frac{1}{2} (\bar c_{uu}^A -\bar c_{dd}^A )\tag{1.1}\\
c_\eta (\theta_{\eta a} + \theta_{a \eta}-\theta_{\pi^0\eta}\theta_{\eta a}) + s_\eta (\theta_{\eta' a}+\theta_{a\eta'}-\theta_{\pi^0 \eta'}\theta_{\eta' a})&= \frac{1}{2\sqrt{3}}(\bar{c}_{uu}^A +\bar c_{dd}^A -2 \bar c_{ss}^A)  \tag{1.2}\\
-s_\eta (\theta_{\eta a} + \theta_{a \eta}-\theta_{\pi^0\eta}\theta_{\eta a}) + c_\eta (\theta_{\eta' a}+\theta_{a\eta'}-\theta_{\pi^0 \eta'}\theta_{\eta' a})&= \frac{1}{\sqrt{6}}(\bar{c}_{uu}^A +\bar c_{dd}^A + \bar c_{ss}^A)  \tag{1.3}\\
\theta_{\bar K^0 a} + \theta_{a K^0} &= \frac{1}{\sqrt{2}}\bar c_{sd}^A\tag{1.4}\\
\theta_{K^0 a} + \theta_{a \bar K^0} &= \frac{1}{\sqrt{2}}\bar c_{ds}^A\tag{1.5}\\
\theta_{\pi^0 a}^2 + \theta_{\eta a}^2 + \theta_{\eta' a}^2 + 2 \theta_{K^0 a}\theta_{\bar K^0 a} + 2\theta_{aa} &= \frac{1}{2}[(\bar c_{uu}^A)^2 + (\bar c_{dd}^A)^2 + (\bar c_{ss}^A)^2 + 2 \bar c_{ds}^A \bar c_{sd}^A] \tag{1.6}\\
-(m_a^2 \theta_{a\pi^0}+m_\pi^2 \theta_{\pi^0 a}+ m_\eta^2 \theta_{\pi^0\eta}\theta_{\eta a}+ m_{\eta'}^2 \theta_{\pi^0\eta'}\theta_{\eta' a})\frac{\langle a\rangle}{f_a} &=\frac{1}{2} \left[\sin(\alpha_u - 2\varphi_{uu})(m_{\bar K}^2 - \Delta^2 + \epsilon_I) - c_{u_0}^2\sin(\alpha_d - 2\varphi_{dd}) (m_{\bar K}^2 -\Delta^2 -\epsilon_I) + s_{u_0}^2\sin(\alpha_s - \varphi_{dd}-\varphi_{ss})(m_{\bar K}^2 + \Delta^2) \right]\tag{1.7}\\
-[c_\eta(m_a^2 \theta_{a\eta}+m_\eta^2\theta_{\eta a}-m_\pi^2 \theta_{\pi^0\eta}\theta_{\pi^0 a})+s_\eta (m_a^2 \theta_{a\eta'}+m_{\eta'}^2\theta_{\eta a}-m_\pi^2 \theta_{\pi^0\eta'}\theta_{\pi^0 a})]\frac{\langle a\rangle}{f_a}&= \frac{1}{2\sqrt{3}} \left[\sin(\alpha_u - 2\varphi_{uu})(m_{\bar K}^2 -\Delta^2 + \epsilon_I) + c_{u_0}^2 \sin(\alpha_d - 2\varphi_{dd})(m_{\bar K}^2-\Delta^2-\epsilon_I) -2c_{u_0}^2\sin(\alpha_s - 2\varphi_{ss})(m_{\bar K}^2 + \Delta^2)+2s_{u_0}^2 \sin(\alpha_d-\varphi_{dd}-\varphi_{ss})(m_{\bar K}^2-\Delta^2-\epsilon_I) - s_{u_0}^2 \sin(\alpha_s-\varphi_{dd}-\varphi_{ss})(m_{\bar K}^2 + \Delta^2)\right]\tag{1.8}\\
-[s_\eta(m_a^2 \theta_{a\eta}+m_\eta^2\theta_{\eta a}-m_\pi^2 \theta_{\pi^0\eta}\theta_{\pi^0 a})-c_\eta (m_a^2 \theta_{a\eta'}+m_{\eta'}^2\theta_{\eta' a}-m_\pi^2 \theta_{\pi^0\eta'}\theta_{\pi^0 a})]\frac{\langle a \rangle}{f_a}&= -\frac{m_0^2}{\sqrt{6}}(\theta_0 + 2\varphi_{uu}+2\varphi_{dd} + 2\varphi_{ss}) +\frac{1}{\sqrt{6}}\left[\sin(\alpha_u - 2\varphi_{uu})(m_{\bar K}^2 -\Delta^2 + \epsilon_I) + c_{u_0}^2 \sin(\alpha_d - 2\varphi_{dd})(m_{\bar K}^2-\Delta^2-\epsilon_I) +c_{u_0}^2\sin(\alpha_s - 2\varphi_{ss})(m_{\bar K}^2 + \Delta^2)-s_{u_0}^2 \sin(\alpha_d-\varphi_{dd}-\varphi_{ss})(m_{\bar K}^2-\Delta^2-\epsilon_I) - s_{u_0}^2 \sin(\alpha_s-\varphi_{dd}-\varphi_{ss})(m_{\bar K}^2 + \Delta^2)\right]\tag{1.9}\\
-(m_a^2 \theta_{aK^0} + m_{K^0}^2 \theta_{\bar K^0 a})\frac{\langle a\rangle}{f_a} &= \frac{i}{\sqrt{2}}s_{u_0} c_{u_0}\left[\cos(\alpha_d - 3 \varphi_{dd}/2-\varphi_{ss}/2)(m_{\bar K}^2-\Delta^2-\epsilon_I) + \cos(\alpha_s - \varphi_{dd}/2 -3\varphi_{ss}/2)(m_{\bar K}^2 +\Delta^2)\right] e^{i \Delta_{sd}/2}\tag{1.10}\\
-(m_a^2 \theta_{a\bar K^0} + m_{K^0}^2)\frac{\langle a\rangle}{f_a} &= - \frac{i}{\sqrt{2}}s_{u_0} c_{u_0}\left[\cos(\alpha_d - 3 \varphi_{dd}/2-\varphi_{ss}/2)(m_{\bar K}^2-\Delta^2-\epsilon_I) + \cos(\alpha_s - \varphi_{dd}/2 -3\varphi_{ss}/2)(m_{\bar K}^2 +\Delta^2)\right] e^{-i \Delta_{sd}/2}\tag{1.11}\\
- m_a^2 \frac{\langle a\rangle}{f_a} &=  \frac{c_G F_0^2 m_0^2}{3 f_a^2}(\theta_0 + 2\varphi_{uu}+2\varphi_{dd} + 2\varphi_{ss})\tag{1.12} \\
m_\pi^2 &= \frac{1}{2}\left[\cos(\alpha_u -2\varphi_{uu})(m_{\bar K}^2 -\Delta^2+\epsilon_I)+c_{u_0}^2\cos(\alpha_d-2\varphi_{dd})(m_{\bar K}^2-\Delta^2-\epsilon_I)-s_{u_0}^2\cos(\alpha_s-\varphi_{dd}-\varphi_{ss})(m_{\bar K}^2 + \Delta^2)\right]\tag{1.13}\\
c_\eta^2 m_\eta^2 + s_\eta^2 m_{\eta'}^2 &= \frac{1}{6}\left[\cos(\alpha_u-2\varphi_{uu})(m_{\bar K}^2 -\Delta^2 +\epsilon_I)+c_{u_0}^2 \cos(\alpha_d-2\varphi_{dd}) (m_{\bar K}^2-\Delta^2-\epsilon_I)+4c_{u_0}^2 \cos(\alpha_s-2\varphi_{ss})(m_{\bar K}^ 2+\Delta^2)-4s_{u_0}^2 \cos(\alpha_d-\varphi_{dd}-\varphi_{ss})(m_{\bar K}^2-\Delta^2-\epsilon_I)-s_{u_0}^2\cos(\alpha_s - \varphi_{dd}-\varphi_{ss})(m_{\bar K}^2+\Delta^2)\right]\tag{1.14}\\
s_\eta^2 m_\eta^2 + c_\eta^2 m_{\eta'}^2 &= m_0^2 + \frac{1}{3}\left[\cos(\alpha_u-2\varphi_{uu})(m_{\bar K}^2 -\Delta^2 +\epsilon_I)+c_{u_0}^2 \cos(\alpha_d-2\varphi_{dd}) (m_{\bar K}^2-\Delta^2-\epsilon_I)+c_{u_0}^2 \cos(\alpha_s-2\varphi_{ss})(m_{\bar K}^ 2+\Delta^2)-s_{u_0}^2 \cos(\alpha_d-\varphi_{dd}-\varphi_{ss})(m_{\bar K}^2-\Delta^2-\epsilon_I)-s_{u_0}^2\cos(\alpha_s - \varphi_{dd}-\varphi_{ss})(m_{\bar K}^2+\Delta^2)\right]\tag{1.15}\\
m_{K^0}^2 &= \frac{1}{2}\left[c_{u_0}^2 \cos(\alpha_d-2\varphi_{dd})(m_{\bar K}^2 -\Delta^2 -\epsilon_I)+c_{u_0}^2\cos(\alpha_s-2\varphi_{ss})(m_{\bar K}^2+\Delta^2)-s_{u_0}^2 \cos(\alpha_d-\varphi_{dd}-\varphi_{ss})(m_{\bar K}^2 -\Delta^2 -\epsilon_I)-s_{u_0}^2\cos(\alpha_s-\varphi_{dd}-\varphi_{ss})(m_{\bar K}^2+\Delta^2)\right]\tag{1.16}\\
m_{K^\pm}^2 &= \frac{1}{2}\left[\cos(\alpha_u-2\varphi_{uu})(m_{\bar K}^2-\Delta^2+\epsilon_I)+c_{u_0}^2\cos(\alpha_s-2\varphi_{ss})(m_{\bar K}^2+\Delta^2)-s_{u_0}^2\cos(\alpha_d-\varphi_{dd}-\varphi_{ss})(m_{\bar K}^2-\Delta^2-\epsilon_I)\right]\tag{1.17}\\
c_\eta(m_\pi^2-m_\eta^2)\theta_{\pi^0\eta} + s_\eta (m_\pi^2-m_{\eta'}^2)\theta_{\pi^0\eta'} &= -\frac{1}{2\sqrt{3}}\left[\cos(\alpha_u-2\varphi_{uu})(m_{\bar K}^2-\Delta^2+\epsilon_I)-c_{u_0}^2\cos(\alpha_d-2\varphi_{dd})(m_{\bar K}^2-\Delta^2-\epsilon_I)+s_{u_0}^2\cos(\alpha_s-\varphi_{dd}-\varphi_{ss})(m_{\bar K}^2+\Delta^2)\right]\tag{1.18}\\
-s_\eta(m_\pi^2-m_\eta^2)\theta_{\pi^0\eta} + c_\eta (m_\pi^2-m_{\eta'}^2)\theta_{\pi^0\eta'} &= -\frac{1}{\sqrt{6}}\left[\cos(\alpha_u-2\varphi_{uu})(m_{\bar K}^2-\Delta^2+\epsilon_I)-c_{u_0}^2\cos(\alpha_d-2\varphi_{dd})(m_{\bar K}^2-\Delta^2-\epsilon_I)+s_{u_0}^2\cos(\alpha_s-\varphi_{dd}-\varphi_{ss})(m_{\bar K}^2+\Delta^2)\right]\tag{1.19}\\
(m_\eta^2-m_{\eta'}^2)s_\eta c_\eta &= -\frac{1}{3\sqrt{2}}\left[\cos(\alpha_u-2\varphi_{uu})(m_{\bar K}^2-\Delta^2+\epsilon_I)+c_{u_0}^2\cos(\alpha_d-2\varphi_{dd})(m_{\bar K}^2-\Delta^2-\epsilon_I)-2c_{u_0}^2\cos(\alpha_s-2\varphi_{ss})(m_{\bar K}^2+\Delta^2)+2s_{u_0}^2\cos(\alpha_d-\varphi_{dd}-\varphi_{ss})(m_{\bar K}^2-\Delta^2-\epsilon_I)-s_{u_0}^2\cos(\alpha_s-\varphi_{dd}-\varphi_{ss})(m_{\bar K}^2+\Delta^2)\right]\tag{1.20}\\
0 &= s_{u_0}c_{u_0}\left[\sin(\alpha_d-3\varphi_{dd}/2-\varphi_{ss}/2)(m_{\bar K}^2-\Delta^2-\epsilon_I)+\sin(\alpha_s-\varphi_{dd}/2-3\varphi_{ss}/2)(m_{\bar K}^2+\Delta^2)\right]\tag{1.21}\\
m_a^2 + \frac{F_0^2}{f_a^2}( m_\pi^2 \theta_{\pi^0a}^2 + m_\eta^2 \theta_{\eta a}^2 + m_{\eta'}^2\theta_{\eta' a}^2 + 2 m_{K^0}^2 \theta_{K^0 a}\theta_{\bar K^0 a}+ 2 m_a^2\theta_{aa}) &= \mu_a^2 + \frac{2 c_G^2 F_0^2 m_0^2}{3f_a^2}\tag{1.22}\\
m_a^2 \theta_{a\pi^0} + m_{\pi}^2 \theta_{\pi^0 a} + m_\eta^2 \theta_{\pi^0\eta}\theta_{\eta a} + m_{\eta'}^2 \theta_{\pi^0 \eta'} \theta_{\eta' a} &=0\tag{1.23}\\
 c_\eta(m_a^2 \theta_{a\eta}+m_\eta^2\theta_{\eta a}-m_\pi^2 \theta_{\pi^0\eta}\theta_{\pi^0 a})+s_\eta (m_a^2 \theta_{a\eta'}+m_{\eta'}^2\theta_{\eta a}-m_\pi^2 \theta_{\pi^0\eta'}\theta_{\pi^0 a}) &= 0\tag{1.24}\\
 -s_\eta(m_a^2 \theta_{a\eta}+m_\eta^2\theta_{\eta a}-m_\pi^2 \theta_{\pi^0\eta}\theta_{\pi^0 a})+c_\eta (m_a^2 \theta_{a\eta'}+m_{\eta'}^2\theta_{\eta' a}-m_\pi^2 \theta_{\pi^0\eta'}\theta_{\pi^0 a}) &= \sqrt{\frac{2}{3}}c_G m_0^2\tag{1.25} \\
 m_a^2 \theta_{aK^0} + m_{K^0}^2 \theta_{\bar K^0 a} &= 0\tag{1.26}\\
 m_a^2 \theta_{a\bar K^0} + m_{K^0}^2 \theta_{ K^0 a} &= 0 \tag{1.27}
\end{align}$$
Using eqs.(1.23)-(1.27), we have

$$
\begin{align}
0 &=\frac{1}{2} \left[\sin(\alpha_u - 2\varphi_{uu})(m_{\bar K}^2 - \Delta^2 + \epsilon_I) - c_{u_0}^2\sin(\alpha_d - 2\varphi_{dd}) (m_{\bar K}^2 -\Delta^2 -\epsilon_I) + s_{u_0}^2\sin(\alpha_s - \varphi_{dd}-\varphi_{ss})(m_{\bar K}^2 + \Delta^2) \right]\tag{1.7b}\\
0&= \frac{1}{2\sqrt{3}} \left[\sin(\alpha_u - 2\varphi_{uu})(m_{\bar K}^2 -\Delta^2 + \epsilon_I) + c_{u_0}^2 \sin(\alpha_d - 2\varphi_{dd})(m_{\bar K}^2-\Delta^2-\epsilon_I) -2c_{u_0}^2\sin(\alpha_s - 2\varphi_{ss})(m_{\bar K}^2 + \Delta^2)+2s_{u_0}^2 \sin(\alpha_d-\varphi_{dd}-\varphi_{ss})(m_{\bar K}^2-\Delta^2-\epsilon_I) - s_{u_0}^2 \sin(\alpha_s-\varphi_{dd}-\varphi_{ss})(m_{\bar K}^2 + \Delta^2)\right]\tag{1.8b}\\
\sqrt{\frac{2}{3}}c_G m_0^2\frac{\langle a \rangle}{f_a}&= -\frac{m_0^2}{\sqrt{6}}(\theta_0 + 2\varphi_{uu}+2\varphi_{dd} + 2\varphi_{ss}) +\frac{1}{\sqrt{6}}\left[\sin(\alpha_u - 2\varphi_{uu})(m_{\bar K}^2 -\Delta^2 + \epsilon_I) + c_{u_0}^2 \sin(\alpha_d - 2\varphi_{dd})(m_{\bar K}^2-\Delta^2-\epsilon_I) +c_{u_0}^2\sin(\alpha_s - 2\varphi_{ss})(m_{\bar K}^2 + \Delta^2)-s_{u_0}^2 \sin(\alpha_d-\varphi_{dd}-\varphi_{ss})(m_{\bar K}^2-\Delta^2-\epsilon_I) - s_{u_0}^2 \sin(\alpha_s-\varphi_{dd}-\varphi_{ss})(m_{\bar K}^2 + \Delta^2)\right]\tag{1.9b}\\
0 &=s_{u_0} c_{u_0}\left[\cos(\alpha_d - 3 \varphi_{dd}/2-\varphi_{ss}/2)(m_{\bar K}^2-\Delta^2-\epsilon_I) + \cos(\alpha_s - \varphi_{dd}/2 -3\varphi_{ss}/2)(m_{\bar K}^2 +\Delta^2)\right]\tag{1.10b}\\
\end{align}
$$

Combining eq.(1.22) and eq.(1.10b) we can see that $s_{u_0} c_{u_0}=0$. In order to reproduce the correct vev for the case of only diagonal couplings, we must choose $s_{u_0}=0$, $c_{u_0}=1$, $\boldsymbol{u_0} = \exp(i\boldsymbol{\varphi})$

$$\begin{align}
\bar c^A_{uu} &= c^A_{uu}\\
\bar c^A_{dd} &= c_{dd}^A \\
\bar c_{ss}^A &= c_{ss}^A \\
\bar c_{ds}^A &=  \cos(\varphi_{dd}-\varphi_{ss}) c_{ds}^A + i\sin(\varphi_{dd}-\varphi_{ss})c_{ds}^V\\
\bar c_{sd}^A &=  \cos(\varphi_{dd}-\varphi_{ss})c_{sd}^A - i \sin(\varphi_{dd}-\varphi_{ss})c_{sd}^V
\end{align}$$

$$\begin{align}
\theta_{\pi^0 a} + \theta_{a \pi^0} + \theta_{\pi^0\eta}\theta_{\eta a} + \theta_{\pi^0 \eta'}\theta_{\eta' a} &= \frac{1}{2} ( c_{uu}^A -c_{dd}^A )\tag{1.1c}\\
c_\eta (\theta_{\eta a} + \theta_{a \eta}-\theta_{\pi^0\eta}\theta_{\eta a}) + s_\eta (\theta_{\eta' a}+\theta_{a\eta'}-\theta_{\pi^0 \eta'}\theta_{\eta' a})&= \frac{1}{2\sqrt{3}}(c_{uu}^A +c_{dd}^A -2  c_{ss}^A)  \tag{1.2c}\\
-s_\eta (\theta_{\eta a} + \theta_{a \eta}-\theta_{\pi^0\eta}\theta_{\eta a}) + c_\eta (\theta_{\eta' a}+\theta_{a\eta'}-\theta_{\pi^0 \eta'}\theta_{\eta' a})&= \frac{1}{\sqrt{6}}(c_{uu}^A + c_{dd}^A + c_{ss}^A)  \tag{1.3c}\\
\theta_{\bar K^0 a} + \theta_{a K^0} &= \frac{1}{\sqrt{2}}\bar c_{sd}^A=\frac{1}{\sqrt{2}}[ \cos(\varphi_{dd}-\varphi_{ss}) c_{ds}^A + i\sin(\varphi_{dd}-\varphi_{ss})c_{ds}^V]\tag{1.4c}\\
\theta_{K^0 a} + \theta_{a \bar K^0} &= \frac{1}{\sqrt{2}}\bar c_{ds}^A = \frac{1}{\sqrt{2}}[ \cos(\varphi_{dd}-\varphi_{ss}) c_{ds}^A - i\sin(\varphi_{dd}-\varphi_{ss})c_{ds}^V]\tag{1.5c}\\
\theta_{\pi^0 a}^2 + \theta_{\eta a}^2 + \theta_{\eta' a}^2 + 2 \theta_{K^0 a}\theta_{\bar K^0 a} + 2\theta_{aa} &= \frac{1}{2}[( c_{uu}^A)^2 + ( c_{dd}^A)^2 + (c_{ss}^A)^2 + 2 \bar c_{ds}^A \bar c_{sd}^A] = \frac{1}{2}[( c_{uu}^A)^2 + ( c_{dd}^A)^2 + (c_{ss}^A)^2 + \cos^2(\varphi_{dd}-\varphi_{ss})|c_{ds}^A|^2+\sin^2(\varphi_{dd}-\varphi_{ss})|c_{ds}^V|^2+\sin(2\varphi_{dd}-2\varphi_{ss})(\mathrm{Im}\,c_{ds}^A\ \mathrm{Re}\,c_{ds}^V-\mathrm{Re}\,c_{ds}^A\ \mathrm{Im}\,c_{ds}^V)]\tag{1.6c} \\
0 &=\frac{1}{2} \left[\sin(\alpha_u - 2\varphi_{uu})(m_{\bar K}^2 - \Delta^2 + \epsilon_I) - \sin(\alpha_d - 2\varphi_{dd}) (m_{\bar K}^2 -\Delta^2 -\epsilon_I) \right]\tag{1.7c}\\
0 &= \frac{1}{2\sqrt{3}} \left[\sin(\alpha_u - 2\varphi_{uu})(m_{\bar K}^2 -\Delta^2 + \epsilon_I) + \sin(\alpha_d - 2\varphi_{dd})(m_{\bar K}^2-\Delta^2-\epsilon_I) -2\sin(\alpha_s - 2\varphi_{ss})(m_{\bar K}^2 + \Delta^2)\right]\tag{1.8c}\\
\sqrt{\frac{2}{3}}c_G m_0^2\frac{\langle a \rangle}{f_a}&= -\frac{m_0^2}{\sqrt{6}}(\theta_0 + 2\varphi_{uu}+2\varphi_{dd} + 2\varphi_{ss}) +\frac{1}{\sqrt{6}}\left[\sin(\alpha_u - 2\varphi_{uu})(m_{\bar K}^2 -\Delta^2 + \epsilon_I) +  \sin(\alpha_d - 2\varphi_{dd})(m_{\bar K}^2-\Delta^2-\epsilon_I) +\sin(\alpha_s - 2\varphi_{ss})(m_{\bar K}^2 + \Delta^2)\right]\tag{1.9c}\\
- m_a^2 \frac{\langle a\rangle}{f_a} &=  \frac{c_G F_0^2 m_0^2}{3 f_a^2}(\theta_0 + 2\varphi_{uu}+2\varphi_{dd} + 2\varphi_{ss})\tag{1.12c} \\
m_{\pi}^2 &= \frac{1}{2}\left[\cos(\alpha_u -2\varphi_{uu})(m_{\bar K}^2 -\Delta^2+\epsilon_I)+\cos(\alpha_d-2\varphi_{dd})(m_{\bar K}^2-\Delta^2-\epsilon_I)\right]\tag{1.13c}\\
c_\eta^2 m_\eta^2 + s_\eta^2 m_{\eta'}^2 &= \frac{1}{6}\left[\cos(\alpha_u-2\varphi_{uu})(m_{\bar K}^2 -\Delta^2 +\epsilon_I)+ \cos(\alpha_d-2\varphi_{dd}) (m_{\bar K}^2-\Delta^2-\epsilon_I)+4 \cos(\alpha_s-2\varphi_{ss})(m_{\bar K}^ 2+\Delta^2)\right]\tag{1.14c}\\
s_\eta^2 m_\eta^2 + c_\eta^2 m_{\eta'}^2 &= m_0^2 + \frac{1}{3}\left[\cos(\alpha_u-2\varphi_{uu})(m_{\bar K}^2 -\Delta^2 +\epsilon_I)+ \cos(\alpha_d-2\varphi_{dd}) (m_{\bar K}^2-\Delta^2-\epsilon_I)+ \cos(\alpha_s-2\varphi_{ss})(m_{\bar K}^ 2+\Delta^2)\right]\tag{1.15c}\\
m_{K^0}^2 &= \frac{1}{2}\left[\cos(\alpha_d-2\varphi_{dd})(m_{\bar K}^2 -\Delta^2 -\epsilon_I)+\cos(\alpha_s-2\varphi_{ss})(m_{\bar K}^2+\Delta^2)\right]\tag{1.16c}\\
m_{K^\pm}^2 &= \frac{1}{2}\left[\cos(\alpha_u-2\varphi_{uu})(m_{\bar K}^2-\Delta^2+\epsilon_I)+\cos(\alpha_s-2\varphi_{ss})(m_{\bar K}^2+\Delta^2)\right]\tag{1.17c}\\
c_\eta(m_\pi^2-m_\eta^2)\theta_{\pi^0\eta} + s_\eta (m_\pi^2-m_{\eta'}^2)\theta_{\pi^0\eta'} &= -\frac{1}{2\sqrt{3}}\left[\cos(\alpha_u-2\varphi_{uu})(m_{\bar K}^2-\Delta^2+\epsilon_I)-\cos(\alpha_d-2\varphi_{dd})(m_{\bar K}^2-\Delta^2-\epsilon_I)\right]\tag{1.18c}\\
-s_\eta(m_\pi^2-m_\eta^2)\theta_{\pi^0\eta} + c_\eta (m_\pi^2-m_{\eta'}^2)\theta_{\pi^0\eta'} &= -\frac{1}{\sqrt{6}}\left[\cos(\alpha_u-2\varphi_{uu})(m_{\bar K}^2-\Delta^2+\epsilon_I)-\cos(\alpha_d-2\varphi_{dd})(m_{\bar K}^2-\Delta^2-\epsilon_I)\right]\tag{1.19c}\\
(m_\eta^2-m_{\eta'}^2)s_\eta c_\eta &= -\frac{1}{3\sqrt{2}}\left[\cos(\alpha_u-2\varphi_{uu})(m_{\bar K}^2-\Delta^2+\epsilon_I)+\cos(\alpha_d-2\varphi_{dd})(m_{\bar K}^2-\Delta^2-\epsilon_I)-2\cos(\alpha_s-2\varphi_{ss})(m_{\bar K}^2+\Delta^2)\right]\tag{1.20c}\\
m_a^2 + \frac{F_0^2}{f_a^2}( m_\pi^2 \theta_{\pi^0a}^2 + m_\eta^2 \theta_{\eta a}^2 + m_{\eta'}^2\theta_{\eta' a}^2 + 2 m_{K^0}^2 \theta_{K^0 a}\theta_{\bar K^0 a}+ 2 m_a^2\theta_{aa}) &= \mu_a^2 + \frac{2 c_G^2 F_0^2 m_0^2}{3f_a^2}\tag{1.22c}\\
 m_a^2 \theta_{a\pi^0} + m_{\pi}^2 \theta_{\pi^0 a} + m_\eta^2 \theta_{\pi^0\eta}\theta_{\eta a} + m_{\eta'}^2 \theta_{\pi^0 \eta'} \theta_{\eta' a} &=0\tag{1.23c}\\
 c_\eta(m_a^2 \theta_{a\eta}+m_\eta^2\theta_{\eta a}-m_\pi^2 \theta_{\pi^0\eta}\theta_{\pi^0 a})+s_\eta (m_a^2 \theta_{a\eta'}+m_{\eta'}^2\theta_{\eta a}-m_\pi^2 \theta_{\pi^0\eta'}\theta_{\pi^0 a}) &= 0\tag{1.24c}\\
 -s_\eta(m_a^2 \theta_{a\eta}+m_\eta^2\theta_{\eta a}-m_\pi^2 \theta_{\pi^0\eta}\theta_{\pi^0 a})+c_\eta (m_a^2 \theta_{a\eta'}+m_{\eta'}^2\theta_{\eta' a}-m_\pi^2 \theta_{\pi^0\eta'}\theta_{\pi^0 a}) &= \sqrt{\frac{2}{3}}c_G m_0^2 \tag{1.25c}\\
 m_a^2 \theta_{aK^0} + m_{K^0}^2 \theta_{\bar K^0 a} &= 0 \tag{1.26c}\\
 m_a^2 \theta_{a\bar K^0} + m_{K^0}^2 \theta_{ K^0 a} &= 0 \tag{1.27c}
\end{align}$$

Plugging (1.12c) into (1.9c)

$$
-\frac{m_0^2}{\sqrt{6}}\frac{2 c_G^2 F_0^2 m_0^2}{3f_a^2 m_a^2}(\theta_0 + 2\varphi_{uu}+2\varphi_{dd} + 2\varphi_{ss}) = -\frac{m_0^2}{\sqrt{6}}(\theta_0 + 2\varphi_{uu}+2\varphi_{dd} + 2\varphi_{ss}) +\frac{1}{\sqrt{6}}\left[\sin(\alpha_u - 2\varphi_{uu})(m_{\bar K}^2 -\Delta^2 + \epsilon_I) +  \sin(\alpha_d - 2\varphi_{dd})(m_{\bar K}^2-\Delta^2-\epsilon_I) +\sin(\alpha_s - 2\varphi_{ss})(m_{\bar K}^2 + \Delta^2)\right]\tag{1.9d}
$$

With eq.(1.7c), (1.8c) and (1.9c) we can obtain the phases of the vev matrix. The first two equations tell us
$$m_u \sin\bar\varphi_u= m_d \sin\bar\varphi_{d} = m_s \sin\bar\varphi_{s}$$ where $\bar\varphi_q = \alpha_q-2\varphi_{qq}\ll1$. With the third equation, we obtain the Dashen-Nuyts condition[^3]
$$\begin{align}
m_0^2 \left(1 - \frac{2 c_G^2 F_0^2 m_0^2}{3f_a^2 m_a^2}\right)(\bar \theta -\bar\varphi_u-\bar\varphi_d-\bar\varphi_s) &= 2 B_0(m_u \sin\bar\varphi_u+ m_d \sin\bar\varphi_{d} + m_s \sin\bar\varphi_{s})\\
m_0^2 \left(1 - \frac{2 c_G^2 F_0^2 m_0^2}{3f_a^2 m_a^2}\right)\left[\bar\theta -m_u\bar \varphi_u \left(\frac{1}{m_u}+\frac{1}{m_d}+\frac{1}{m_s}\right)\right] &\approx6 B_0 m_u \bar\varphi_u
\end{align}$$
$$
\boldsymbol{\bar\varphi} = \frac{m_0^2 \left(1 - \frac{2 c_G^2 F_0^2 m_0^2}{3f_a^2 m_a^2}\right)}{6 B_0 + 2 m_0^2 \left(1 - \frac{2 c_G^2 F_0^2 m_0^2}{3f_a^2 m_a^2}\right)\langle|\boldsymbol{m_q}|^{-1}\rangle} |\boldsymbol{m_q}|^{-1} \bar\theta \equiv \widetilde m |\boldsymbol{m_q}|^{-1} \bar\theta 
$$
$$\boldsymbol{u_0} = \exp(i \boldsymbol{\varphi}) = \exp\left(i\frac{\boldsymbol{\alpha }- \boldsymbol{\bar \varphi}}{2}\right)\approx \exp\left(i\frac{\boldsymbol{\alpha }}{2}\right)\left(\boldsymbol{1}-\frac{i}{2}\widetilde m |\boldsymbol{m_q}|^{-1} \bar\theta \right)$$
$$\boldsymbol{\bar m_q}  = \boldsymbol{u_0}^\dagger \boldsymbol{m_q}\boldsymbol{u_0}^\dagger = |\boldsymbol{m_q}|-i\widetilde m \bar \theta \boldsymbol{1}$$

$$\mathcal{L}_\chi = F_0^2 B_0 \langle \boldsymbol{\bar m_q}^\dagger \boldsymbol{\bar U} +  \boldsymbol{\bar m_q} \boldsymbol{\bar U}^\dagger\rangle = F_0^2 B_0 \langle |\boldsymbol{m_q}|(\boldsymbol{\bar U} + \boldsymbol{\bar U}^\dagger)\rangle + iF_0^2 B_0 \widetilde m\bar \theta \langle \boldsymbol{\bar U}-\boldsymbol{\bar U}^\dagger\rangle$$

Now we can approximate $\cos(\alpha_q-2\varphi_{qq}) \approx 1$, which allows us to disentangle some of the purely-SM constraints:

$$\begin{align}
m_{\pi}^2 &= \frac{1}{2}\left[(m_{\bar K}^2 -\Delta^2+\epsilon_I)+(m_{\bar K}^2-\Delta^2-\epsilon_I)\right]= m_{\bar K}^2-\Delta^2 \tag{1.13d}\\
c_\eta^2 m_\eta^2 + s_\eta^2 m_{\eta'}^2 &= \frac{1}{6}\left[(m_{\bar K}^2 -\Delta^2 +\epsilon_I)+  (m_{\bar K}^2-\Delta^2-\epsilon_I)+4(m_{\bar K}^ 2+\Delta^2)\right] = m_{\bar K}^2+\frac{1}{3}\Delta^2\tag{1.14d}\\
s_\eta^2 m_\eta^2 + c_\eta^2 m_{\eta'}^2 &= m_0^2 + \frac{1}{3}\left[(m_{\bar K}^2 -\Delta^2 +\epsilon_I)+  (m_{\bar K}^2-\Delta^2-\epsilon_I)+(m_{\bar K}^ 2+\Delta^2)\right]=m_0^2+m_{\bar K}^2-\frac{1}{3}\Delta^2\tag{1.15d}\\
m_{K^0}^2 &= \frac{1}{2}\left[(m_{\bar K}^2 -\Delta^2 -\epsilon_I)+(m_{\bar K}^2+\Delta^2)\right]=m_{\bar K}^2-\frac{1}{2}\epsilon_I\tag{1.16d}\\
m_{K^\pm}^2 &= \frac{1}{2}\left[(m_{\bar K}^2-\Delta^2+\epsilon_I)+(m_{\bar K}^2+\Delta^2)\right]=m_{\bar K}^2+\frac{1}{2}\epsilon_I\tag{1.17d}\\
c_\eta(m_\pi^2-m_\eta^2)\theta_{\pi^0\eta} + s_\eta (m_\pi^2-m_{\eta'}^2)\theta_{\pi^0\eta'} &= -\frac{1}{2\sqrt{3}}\left[(m_{\bar K}^2-\Delta^2+\epsilon_I)-(m_{\bar K}^2-\Delta^2-\epsilon_I)\right]=-\frac{\epsilon_I}{\sqrt{3}}\tag{1.18d}\\
-s_\eta(m_\pi^2-m_\eta^2)\theta_{\pi^0\eta} + c_\eta (m_\pi^2-m_{\eta'}^2)\theta_{\pi^0\eta'} &= -\frac{1}{\sqrt{6}}\left[(m_{\bar K}^2-\Delta^2+\epsilon_I)-(m_{\bar K}^2-\Delta^2-\epsilon_I)\right]=-\frac{2\epsilon_I}{\sqrt{6}}\tag{1.19d}\\
(m_\eta^2-m_{\eta'}^2)s_\eta c_\eta &= -\frac{1}{3\sqrt{2}}\left[(m_{\bar K}^2-\Delta^2+\epsilon_I)+(m_{\bar K}^2-\Delta^2-\epsilon_I)-2(m_{\bar K}^2+\Delta^2)\right]=\frac{2\sqrt{2}\Delta^2}{3}\tag{1.20d}\\
\end{align}$$

The $\eta-\eta'$ mixing in eqs.(1.14d), (1.15d) and (1.20d) is solved as
$$\begin{align}
m_\eta^2 &= m_{\bar{K}}^2 + \frac{1}{2}m_0^2 - \frac{1}{2}\sqrt{m_0^4 -\frac{4}{3}m_0^2 \Delta^2 + 4\Delta^4}\\ 
m_{\eta'}^2 &= m_{\bar{K}}^2 + \frac{1}{2}m_0^2 + \frac{1}{2}\sqrt{m_0^4 -\frac{4}{3}m_0^2 \Delta^2 + 4\Delta^4}\\
\sin(2\theta_\eta) &= 2 s_\eta c_\eta = \frac{\frac{4\sqrt{2}}{3}\Delta^2}{\sqrt{m_0^4 -\frac{4}{3} m_0^2 \Delta^2 + 4\Delta^4}}
\end{align}$$

while the $\pi^0-\eta$ and $\pi^0-\eta'$ mixings, eqs.(1.18d) and (1.19d),
$$\begin{align}
\theta_{\pi^0\eta} &=\frac{c_\eta -\sqrt{2}s_\eta}{\sqrt{3}}\frac{\epsilon_I}{m_\eta^2-m_\pi^2}\\
\theta_{\pi^0\eta'} &=\frac{s_\eta +\sqrt{2}c_\eta}{\sqrt{3}}\frac{\epsilon_I}{m_{\eta'}^2-m_\pi^2}
\end{align}$$

The mixing of the ALP with mesons is then described by
$$\begin{align}
\theta_{\pi^0 a} + \theta_{a \pi^0} + \theta_{\pi^0\eta}\theta_{\eta a} + \theta_{\pi^0 \eta'}\theta_{\eta' a} &= \frac{1}{2} ( c_{uu}^A -c_{dd}^A )\tag{1.1d}\\
\theta_{\eta a} + \theta_{a \eta}-\theta_{\pi^0\eta}\theta_{\eta a}&=\frac{1}{2\sqrt{3}}(c_{uu}^A +c_{dd}^A -2  c_{ss}^A)c_\eta-\frac{1}{\sqrt{6}}(c_{uu}^A + c_{dd}^A + c_{ss}^A)s_\eta \tag{1.2d}\\
\theta_{\eta' a}+\theta_{a\eta'}-\theta_{\pi^0 \eta'}\theta_{\eta' a} &=\frac{1}{2\sqrt{3}}(c_{uu}^A +c_{dd}^A -2  c_{ss}^A)s_\eta+\frac{1}{\sqrt{6}}(c_{uu}^A + c_{dd}^A + c_{ss}^A)c_\eta \tag{1.3d}\\
\theta_{\bar K^0 a} + \theta_{a K^0} &= \frac{1}{\sqrt{2}}\bar c_{sd}^A=\frac{1}{\sqrt{2}}[ \cos(\varphi_{dd}-\varphi_{ss}) c_{ds}^A + i\sin(\varphi_{dd}-\varphi_{ss})c_{ds}^V]\tag{1.4d}\\
\theta_{K^0 a} + \theta_{a \bar K^0} &= \frac{1}{\sqrt{2}}\bar c_{ds}^A = \frac{1}{\sqrt{2}}[ \cos(\varphi_{dd}-\varphi_{ss}) c_{ds}^A - i\sin(\varphi_{dd}-\varphi_{ss})c_{ds}^V]\tag{1.5d}\\
\theta_{\pi^0 a}^2 + \theta_{\eta a}^2 + \theta_{\eta' a}^2 + 2 \theta_{K^0 a}\theta_{\bar K^0 a} + 2\theta_{aa} &= \frac{1}{2}[( c_{uu}^A)^2 + ( c_{dd}^A)^2 + (c_{ss}^A)^2 + 2 \bar c_{ds}^A \bar c_{sd}^A] = \frac{1}{2}[( c_{uu}^A)^2 + ( c_{dd}^A)^2 + (c_{ss}^A)^2 + \cos^2(\varphi_{dd}-\varphi_{ss})|c_{ds}^A|^2+\sin^2(\varphi_{dd}-\varphi_{ss})|c_{ds}^V|^2+\sin(2\varphi_{dd}-2\varphi_{ss})(\mathrm{Im}\,c_{ds}^A\ \mathrm{Re}\,c_{ds}^V-\mathrm{Re}\,c_{ds}^A\ \mathrm{Im}\,c_{ds}^V)]\tag{1.6d} \\
 m_a^2 \theta_{a\pi^0} + m_{\pi}^2 \theta_{\pi^0 a} + m_\eta^2 \theta_{\pi^0\eta}\theta_{\eta a} + m_{\eta'}^2 \theta_{\pi^0 \eta'} \theta_{\eta' a} &=0\tag{1.23d}\\
 m_a^2 \theta_{a\eta}+m_\eta^2\theta_{\eta a}-m_\pi^2 \theta_{\pi^0\eta}\theta_{\pi^0 a}&=-\sqrt{\frac{2}{3}}c_G m_0^2s_\eta\tag{1.24d}\\
 m_a^2 \theta_{a\eta'}+m_{\eta'}^2\theta_{\eta a}-m_\pi^2 \theta_{\pi^0\eta'}\theta_{\pi^0 a} &= \sqrt{\frac{2}{3}}c_G m_0^2c_\eta\tag{1.25d}\\
 m_a^2 \theta_{aK^0} + m_{K^0}^2 \theta_{\bar K^0 a} &= 0 \tag{1.26d}\\
 m_a^2 \theta_{a\bar K^0} + m_{K^0}^2 \theta_{ K^0 a} &= 0 \tag{1.27d} 
\end{align}$$

The solution is then
$$\begin{align}
\theta_{\pi^0 a} &= \frac{1}{m_a^2-m_\pi^2} \left[\frac{m_a^2}{2} ( c_{uu}^A -c_{dd}^A )-\theta_{\pi^0 \eta}\left(\sqrt{\frac{2}{3}}c_G m_0^ 2s_\eta +\frac{m_a^2}{2\sqrt{3}}(c_{uu}^A +c_{dd}^A -2  c_{ss}^A)c_\eta-\frac{m_a^2}{\sqrt{6}}(c_{uu}^A + c_{dd}^A + c_{ss}^A)s_\eta\right)-\theta_{\pi^0\eta'}\left(-\sqrt{\frac{2}{3}}c_G m_0^2c_\eta+\frac{m_a^2}{2\sqrt{3}}(c_{uu}^A +c_{dd}^A -2  c_{ss}^A)s_\eta+\frac{m_a^2}{\sqrt{6}}(c_{uu}^A + c_{dd}^A + c_{ss}^A)c_\eta\right)\right]+\mathcal{O}(\epsilon_I^2)\\
\theta_{\eta a} &= \frac{1}{m_a^2-m_\eta^2}\left[\sqrt{\frac{2}{3}}c_G m_0^ 2s_\eta +\frac{m_a^2}{2\sqrt{3}}(c_{uu}^A +c_{dd}^A -2  c_{ss}^A)c_\eta-\frac{m_a^2}{\sqrt{6}}(c_{uu}^A + c_{dd}^A + c_{ss}^A)s_\eta\right]+\mathcal{O}(\epsilon_I)\\
\theta_{\eta' a} &= \frac{1}{m_a^2-m_{\eta'}^2}\left[-\sqrt{\frac{2}{3}}c_G m_0^2c_\eta+\frac{m_a^2}{2\sqrt{3}}(c_{uu}^A +c_{dd}^A -2  c_{ss}^A)s_\eta+\frac{m_a^2}{\sqrt{6}}(c_{uu}^A + c_{dd}^A + c_{ss}^A)c_\eta\right] + \mathcal{O}(\epsilon_I)\\
\theta_{a\pi^0 } &= \frac{1}{m_a^2-m_\pi^2} \left[-\frac{m_\pi^2}{2} ( c_{uu}^A -c_{dd}^A )-\theta_{\pi^0 \eta}\frac{m_\eta^2-m_\pi^2}{m_a^2-m_\eta^2}\left(\sqrt{\frac{2}{3}}c_G m_0^ 2s_\eta +\frac{m_a^2}{2\sqrt{3}}(c_{uu}^A +c_{dd}^A -2  c_{ss}^A)c_\eta-\frac{m_a^2}{\sqrt{6}}(c_{uu}^A + c_{dd}^A + c_{ss}^A)s_\eta\right)-\theta_{\pi^0\eta'}\frac{m_{\eta'}^2-m_\pi^2}{m_a^2-m_{\eta'}^2}\left(-\sqrt{\frac{2}{3}}c_G m_0^2c_\eta+\frac{m_a^2}{2\sqrt{3}}(c_{uu}^A +c_{dd}^A -2  c_{ss}^A)s_\eta+\frac{m_a^2}{\sqrt{6}}(c_{uu}^A + c_{dd}^A + c_{ss}^A)c_\eta\right)\right]+\mathcal{O}(\epsilon_I^2)\\
\theta_{a\eta} &= \frac{-1}{m_a^2-m_\eta^2}\left[\sqrt{\frac{2}{3}}c_G m_0^ 2s_\eta +\frac{m_\eta^2}{2\sqrt{3}}(c_{uu}^A +c_{dd}^A -2  c_{ss}^A)c_\eta-\frac{m_\eta^2}{\sqrt{6}}(c_{uu}^A + c_{dd}^A + c_{ss}^A)s_\eta\right]+\mathcal{O}(\epsilon_I)\\
\theta_{a\eta'} &= \frac{-1}{m_a^2-m_{\eta'}^2}\left[-\sqrt{\frac{2}{3}}c_G m_0^2c_\eta+\frac{m_{\eta'}^2}{2\sqrt{3}}(c_{uu}^A +c_{dd}^A -2  c_{ss}^A)s_\eta+\frac{m_{\eta'}^2}{\sqrt{6}}(c_{uu}^A + c_{dd}^A + c_{ss}^A)c_\eta\right] + \mathcal{O}(\epsilon_I)
\end{align}$$

and the physical mass of the axion is
$$
m_a^2 = \mu_a^2 + \frac{F_0^2}{f_a^2}\left[\frac{2}{3}c_G^2 m_0^2 + (\mu_a^2-m_\pi^2)\theta_{\pi^0 a}^2+ (\mu_a^2-m_\eta^2)\theta_{\eta a}^2 + (\mu_a^2-m_{\eta'}^2)\theta_{\eta' a}^2 + 2(\mu_a^2-m_{K^0}^2)\theta_{K^0 a}\theta_{\bar K^0 a}- \frac{1}{2}[( c_{uu}^A)^2 + ( c_{dd}^A)^2 + (c_{ss}^A)^2 + \cos^2(\varphi_{dd}-\varphi_{ss})|c_{ds}^A|^2+\sin^2(\varphi_{dd}-\varphi_{ss})|c_{ds}^V|^2+\sin(2\varphi_{dd}-2\varphi_{ss})(\mathrm{Im}\,c_{ds}^A\ \mathrm{Re}\,c_{ds}^V-\mathrm{Re}\,c_{ds}^A\ \mathrm{Im}\,c_{ds}^V)] \right]
$$

### Comments so far

- The mixing with kaons depends on **Vector** couplings and on **complex phase of quark masses** !!!???
- For axions with $\mu_a=0$ and derivative couplings, the quadratic term of the potential might have wrong sign
- In the QCD case, $m_a^2 < \frac{2 F_0^2}{3f_a^2}c_G^2 m_0^2$, which means that $\widetilde m \neq 0$. Neutron edm???
	- Other ways to get $\widetilde m = 0$ (not realized in real world):
		- $m_u = 0$: $\bar\varphi_d = \bar \varphi_s = 0$, $\bar \varphi_u=\bar \theta$, $\boldsymbol{\bar m_q}=\mathrm{diag}(0, m_d, m_s)$
		- $m_0 = 0$ with $B_0 \neq 0$

## Interactions with baryons

Now we will employ the CCWZ construction, where

$$\begin{align}
\boldsymbol{U} &= \boldsymbol{\xi_R} \boldsymbol{\xi_L}^\dagger \\
\boldsymbol{\xi_R} &= \boldsymbol{u_0} \boldsymbol{\bar u}\\
\boldsymbol{\xi_L} &= \boldsymbol{u_0}^\dagger \boldsymbol{\bar u}^\dagger\\
\boldsymbol{\bar u} &= \exp\left(\frac{i}{2F_0}\boldsymbol{\Phi}\right)\\
\boldsymbol{\xi}_\mu &=i\left[\boldsymbol{\xi_R}^\dagger(\partial_\mu-i\boldsymbol{R}_\mu)\boldsymbol{\xi_R}-\boldsymbol{\xi_L}^\dagger(\partial_\mu-i\boldsymbol{L}_\mu)\boldsymbol{\xi_L}\right]\\
\boldsymbol{\Gamma}_\mu &=\frac{1}{2}\left[\boldsymbol{\xi_R}^\dagger(\partial_\mu-i\boldsymbol{R}_\mu)\boldsymbol{\xi_R}+\boldsymbol{\xi_L}^\dagger(\partial_\mu-i\boldsymbol{L}_\mu)\boldsymbol{\xi_L}\right]\\
\boldsymbol{\chi_\pm} &= \boldsymbol{\xi_L}^\dagger \boldsymbol{\chi}^\dagger \boldsymbol{\xi_R} \pm \boldsymbol{\xi_R}^\dagger \boldsymbol{\chi} \boldsymbol{\xi_L}\\
\boldsymbol{f^R}_{\mu\nu} &= \partial_\mu \boldsymbol{R}_\nu - \partial_\nu \boldsymbol{R}_\mu - i [\boldsymbol{R}_\mu, \boldsymbol{R}_\nu] \\
\boldsymbol{f^L}_{\mu\nu} &= \partial_\mu \boldsymbol{L}_\nu - \partial_\nu \boldsymbol{L}_\mu - i [\boldsymbol{L}_\mu, \boldsymbol{L}_\nu] \\
\boldsymbol{f^\pm}_{\mu\nu} &=  \boldsymbol{\xi_R}^\dagger \boldsymbol{f^R}_{\mu\nu} \boldsymbol{\xi_R} \pm \boldsymbol{\xi_L}^\dagger \boldsymbol{f^L}_{\mu\nu} \boldsymbol{\xi_L}
\end{align}$$

The baryon octect is
$$
\boldsymbol{B} = \begin{pmatrix}
\frac{1}{\sqrt{2}}\Sigma^0 + \frac{1}{\sqrt{6}}\Lambda & \Sigma^+ & p\\
\Sigma^- & -\frac{1}{\sqrt{2}}\Sigma^0 + \frac{1}{\sqrt{6}}\Lambda & n\\
\Xi^- & \Xi^0 & - \frac{2}{\sqrt{6}}\Lambda
\end{pmatrix}
$$

with covariant derivative
$$D_\mu \boldsymbol{B} = \partial_\mu \boldsymbol{B} + [\boldsymbol{\Gamma}_\mu, \boldsymbol{B}]$$

$$\begin{align}
\mathcal{L}\supset& 2 i\langle \bar{\boldsymbol{B}}\gamma_\mu D^\mu\boldsymbol{B}\rangle - 2 m_B \langle \bar{\boldsymbol{B}}\boldsymbol{B}\rangle\\
&-D \langle \bar{\boldsymbol{B}}\gamma_\mu \gamma_5 \{\boldsymbol{\xi_\mu},\boldsymbol{B} \}\rangle - F\langle\bar{\boldsymbol{B}}\gamma_\mu \gamma_5 [\boldsymbol{\xi_\mu},\boldsymbol{B} ]\rangle  + 2\lambda \langle\bar{\boldsymbol{B}}\gamma_\mu\gamma_5 \boldsymbol{B}\rangle \langle\boldsymbol{\xi^\mu}\rangle\\
&+ 2 b_D \langle\bar{\boldsymbol{B}} \{\boldsymbol{\chi_+},\boldsymbol{B}\}\rangle + 2 b_F \langle\bar{\boldsymbol{B}} [\boldsymbol{\chi_+},\boldsymbol{B}]\rangle + 4 b_0\langle \bar{\boldsymbol{B}}\boldsymbol{B}\rangle\langle\boldsymbol{\chi_+}\rangle\\
&+ 2i \left[\theta_0-2\frac{c_G}{f_a}a-2i\langle \log\boldsymbol{U}\rangle\right]\left(w_{10}\langle \bar{\boldsymbol{B}}\{\boldsymbol{\chi_-},\boldsymbol{B}\}\rangle + w_{11}\langle \bar{\boldsymbol{B}}[\boldsymbol{\chi_-},\boldsymbol{B}]\rangle + 2w_{12}\langle \bar{\boldsymbol{B}}\boldsymbol{B}\rangle\langle \boldsymbol{\chi_-}\rangle\right)\\
&+ 2i \left[\theta_0-2\frac{c_G}{f_a}a-2i\langle \log\boldsymbol{ U}\rangle\right] \left(w_{13}\langle \bar{\boldsymbol{B}}\sigma^{\mu\nu}\gamma_5 \{\boldsymbol{f^+}_{\mu\nu},\boldsymbol{B}\}\rangle + w_{14}\langle \bar{\boldsymbol{B}}\sigma^{\mu\nu}\gamma_5 [\boldsymbol{f^+}_{\mu\nu},\boldsymbol{B}]\rangle+2w_{15} \langle \bar{\boldsymbol{B}}\sigma^{\mu\nu}\gamma_5\boldsymbol{B}\rangle \langle \boldsymbol{f^+}_{\mu\nu}\rangle\right)
\end{align}$$

In addition to the ALP, we also include the photon as an external field,
$$\boldsymbol{R}_\mu = \boldsymbol{c_q^R}\frac{\partial_\mu a}{f_a}-e \boldsymbol{Q}A_\mu\,\qquad \boldsymbol{L}_\mu = \boldsymbol{c_q^L}\frac{\partial_\mu a}{f_a}-e \boldsymbol{Q}A_\mu$$

$$\begin{align}
\boldsymbol{\xi}_\mu &\supset -\frac{1}{F_0}\partial_\mu \boldsymbol{\Phi} - \boldsymbol{\bar c_q^A}\frac{\partial_\mu a}{f_a}-i\frac{e}{F_0}[\boldsymbol{Q},\boldsymbol{\Phi}]A_\mu\\
\boldsymbol{\Gamma}_\mu &\supset -i\boldsymbol{\bar c_q^V}\frac{\partial_\mu a}{2f_a}+ie\boldsymbol{Q}A_\mu\\
\boldsymbol{\chi_+} &\supset 4 B_0 |\boldsymbol{m_q}|-4\frac{B_0 \widetilde m}{F_0}\bar \theta \boldsymbol{\Phi}\\
\boldsymbol{\chi_-} &\supset 4iB_0\widetilde m \bar \theta \boldsymbol{1}+\frac{2iB_0}{F_0}\{|\boldsymbol{m_q}|,\boldsymbol{\Phi}\}\\
\boldsymbol{f^+}_{\mu\nu}&\supset -2 e \boldsymbol{Q}F_{\mu\nu} + \frac{i e}{f_a}[\boldsymbol{Q}, \boldsymbol{\bar c_q^V}](\partial_\mu a A_\nu - \partial_\nu a A_\mu)\\
\boldsymbol{f^-}_{\mu\nu}&\supset - \frac{i e}{f_a}[\boldsymbol{Q}, \boldsymbol{\bar c_q^A}](\partial_\mu a A_\nu - \partial_\nu a A_\mu)
\end{align}$$

The terms of the Lagrangian including neutrons and one pseudoscalar are

$$\begin{align}
\mathcal{L} \supset& \frac{c_{dd}^V - c_{ss}^V}{2f_a} \bar n \gamma^\mu n \partial_\mu a - \sqrt{\frac{3}{2}}\frac{\bar c_{sd}^V}{2f_a}\bar n \gamma^\mu \Lambda \partial_\mu a + \frac{\bar c_{ds}^V}{2f_a}\bar n \gamma^\mu \Sigma^0 \partial_\mu a \\
&+D \bar n \gamma^\mu\gamma_5 n \left(\frac{c_{dd}^A + c_{ss}^A}{2f_a}\partial_\mu a-\frac{1}{2F_0}\partial_\mu \pi^0-\frac{1}{2\sqrt{3}F_0}\partial_\mu \eta_8+\sqrt{\frac{2}{3}}\frac{1}{F_0}\partial_\mu \eta_0\right)-\frac{D}{2\sqrt{3}}\bar{n}\gamma^\mu\gamma_5\Lambda \left(\frac{\bar c_{ds}^A}{\sqrt{2}f_a}\partial_\mu a +\frac{1}{F_0} \partial_\mu K^0\right)-\frac{D}{2} \bar n\gamma^\mu \gamma_5 \Sigma^0 \left(\frac{\bar c_{ds}^A}{\sqrt{2}f_a}\partial_\mu a +\frac{1}{F_0} \partial_\mu K^0\right) +\frac{D}{\sqrt{2}F_0}\bar n \gamma^\mu \gamma_5 p (\partial_\mu \pi^- -ieA_\mu \pi^-) +\frac{D}{\sqrt{2}F_0}\bar n \gamma^\mu \gamma_5 \Sigma^- (\partial_\mu K^+ +ieA_\mu K^+)\\
&+ \frac{F }{2}\bar n \gamma^\mu\gamma_5 n \left(\frac{c_{dd}^A-c_{ss}^A}{f_a}\partial_\mu a-\frac{1}{F_0}\partial_\mu \pi^0+\frac{\sqrt{3}}{F_0}\partial_\mu \eta_8\right)-\frac{\sqrt{3}F}{2}\bar n \gamma^\mu \gamma_5\Lambda \left(\frac{\bar c_{ds}^A}{\sqrt{2}f_a}\partial_\mu a + \frac{1}{F_0}\partial_\mu K^0\right)\frac{F}{2}\bar n \gamma^\mu \gamma_5\Sigma^0 \left(\frac{\bar c_{ds}^A}{\sqrt{2}f_a}\partial_\mu a + \frac{1}{F_0}\partial_\mu K^0\right)+\frac{F}{\sqrt{2}F_0}\bar n \gamma^\mu \gamma_5 p (\partial_\mu \pi^- - ie A_\mu \pi^-)-\frac{F}{\sqrt{2}F_0}\bar n \gamma^\mu \gamma_5 \Sigma^- (\partial_\mu K^+ + i e A_\mu K^+)\\
&-\frac{\lambda}{2}\bar n\gamma^\mu \gamma_5 n \left(\frac{c_{uu}^A + c_{dd}^A + c_{ss}^A}{f_a}\partial_\mu a + \frac{\sqrt{6}}{F_0}\partial_\mu\eta_0\right)\\
&+ \frac{2b_D \widetilde m \bar \theta}{F_0} (\bar n n)\left(\pi^0 + \frac{1}{\sqrt{3}}\eta_8-2\sqrt{\frac{2}{3}}\eta_0\right)+ \frac{2b_D \widetilde m \bar \theta}{\sqrt{3}F_0} (\bar n \Lambda)K^0+ \frac{2b_D \widetilde m \bar \theta}{F_0} (\bar n \Sigma^0)K^0 -\frac{2\sqrt{2}b_D \widetilde m \bar \theta}{F_0} (\bar n p)\pi^- - \frac{2\sqrt{2}b_D \widetilde m \bar \theta}{F_0} (\bar n \Sigma^-)K^+ \\
&+ \frac{2b_F \widetilde m \bar \theta}{F_0} (\bar n n)\left(\pi^0-\sqrt{3}\eta_8\right) + \frac{2\sqrt{3} b_F \widetilde m \bar\theta}{F_0}(\bar n \Lambda)K^0 - \frac{2b_F \widetilde m\bar \theta}{F_0}(\bar n \Sigma^0)K^0 -\frac{2\sqrt{2}b_F \widetilde m \bar \theta}{F_0}(\bar n p)\pi^- + \frac{2\sqrt{2}b_F \widetilde m \bar \theta}{F_0}(\bar n \Sigma^-)K^+\\
&-\frac{2\sqrt{6}b_0 \widetilde m\bar \theta}{F_0}(\bar n n)\eta_0\\
&+\frac{2w_{10}B_0}{F_0} \left[\bar\theta (1+2\widetilde m \langle|\boldsymbol{m_q}|^{-1}\rangle)-\frac{2 c_G}{f_a}a+\frac{\sqrt{6}}{F_0}\eta_0\right]\left[2(\bar n n)\left(-2 F_0 \widetilde m \bar \theta+ m_d \pi^0+\frac{1}{\sqrt{3}}(2m_s-m_d)\eta_8-\sqrt{\frac{2}{3}}(m_d+m_s)\eta_0\right)+\frac{(m_d+m_s)}{\sqrt{3}}(\bar n \Lambda)K^0 + (m_d+m_s)(\bar n\Sigma^0)K^0-\sqrt{2}(m_d+m_u)(\bar n p)\pi^- - \sqrt{2}(m_u+m_s)(\bar n \Sigma^-)K^+\right]\\
&+\frac{2w_{11}B_0}{F_0} \left[\bar\theta (1+2\widetilde m \langle|\boldsymbol{m_q}|^{-1}\rangle)-\frac{2 c_G}{f_a}a+\frac{\sqrt{6}}{F_0}\eta_0\right]\left[2(\bar n n)\left(m_d \pi^0-\frac{1}{\sqrt{3}}(m_d+2m_s)\eta_8-\sqrt{\frac{2}{3}}(m_d-m_s)\eta_0\right)+\sqrt{3}(m_d+m_s)(\bar n \Lambda)K^0-(m_d+m_s)(\bar n \Sigma^0)K^0-\sqrt{2}(m_u+m_d)(\bar n p)\pi^- + \sqrt{2} (m_u+m_s)(\bar n \Sigma^-)K^+\right]\\
&+\frac{4w_{12}B_0}{F_0} \left[\bar\theta (1+2\widetilde m \langle|\boldsymbol{m_q}|^{-1}\rangle)-\frac{2 c_G}{f_a}a+\frac{\sqrt{6}}{F_0}\eta_0\right](\bar n n)\left(-3 F_0 \widetilde m \bar \theta\right)
\end{align}$$

- $c_G \neq 0$, $\mu_a \neq 0$: $$\varphi_i = \alpha_i +\frac{1}{m_{q_i}}\frac{\bar \theta}{4 \frac{B_0}{\mu_a^2}c_G^2 \frac{F_\pi^2}{f_a^2}+ 6 \frac{B_0}{m_0^2} + \mathrm{tr}(|\boldsymbol{m_q}|^{-1}) }$$ $$v_a = -2 \frac{B_0}{\mu_a^2} c_G \frac{F_\pi^2}{f_a}\frac{\bar \theta}{4 \frac{B_0}{\mu_a^2}c_G^2 \frac{F_\pi^2}{f_a^2}+ 6 \frac{B_0}{m_0^2} + \mathrm{tr}(|\boldsymbol{m_q}|^{-1}) }$$
- $c_G \neq 0$, $\mu_a \to 0$: $$\varphi_i = \alpha_i +\mu_a^2\frac{\bar \theta}{4 B_0 m_{q_i}c_G^2 \frac{F_\pi^2}{f_a^2}}$$ $$v_a = -\frac{f_a}{2 c_G}\bar\theta$$
- $c_G \neq 0$, $\mu_a\to \infty$: $$\varphi_i = \alpha_i +\frac{1}{m_{q_i}} \frac{\bar \theta}{6\frac{B_0}{m_0^2}+\mathrm{tr}(|\boldsymbol{m_q}|^{-1})}$$ $$v_a= -2\frac{B_0}{\mu_a^2}c_G\frac{F_\pi^2}{f_a} \frac{\bar \theta}{6\frac{B_0}{m_0^2}+\mathrm{tr}(|\boldsymbol{m_q}|^{-1})}$$

# Footnotes

[^1]: [[Axion-meson mixing in light of recent lattice $η$-$η'$ simulations and their two-photon couplings within $U(3)$ chiral theory (2211.02867v2)]]

[^2]:  To compare with their results, set $c_G=-1/2$, $c^A_u=c^A_d=c^A_s = 0$

[^3]:  <a href="https://inspirehep.net/literature/61166"> Some features of chiral symmetry breaking </a> Roger F. Dashen
DOI: <a href="https://doi.org/10.1103/PhysRevD.3.1879"> 10.1103/PhysRevD.3.1879 </a>
Phys.Rev.D 3 (1971), 1879-1889
<a href="https://inspirehep.net/literature/68965"> Is CP-invariance violation caused by an SU(3) singlet? </a>J. Nuyts
DOI: <a href="https://doi.org/10.1103/PhysRevLett.26.1604"> 10.1103/PhysRevLett.26.1604 </a>, <a href="https://doi.org/10.1103/PhysRevLett.27.361.3"> 10.1103/PhysRevLett.27.361.3 </a>(erratum) Phys.Rev.Lett. 26 (1971), 1604-1605
