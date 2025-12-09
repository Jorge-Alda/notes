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

Since the ALP can potentially mix with kaons, let us assume a more generic structure for the vev of $U$,

$$u_0 = \begin{pmatrix}\exp(i \varphi_{uu}) & 0 & 0\\ 0 & c_{u_0} \exp(i\varphi_{dd}) & -s_{u_0}\exp[i(\varphi_{dd} + \varphi_{ss}-\Delta_{sd})/2] \\ 0 & s_{u_0}\exp[i(\varphi_{dd} + \varphi_{ss}+\Delta_{sd})/2] & c_{u_0} \exp(i\varphi_{ss}) \end{pmatrix}$$

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

$$\begin{pmatrix}\pi^0_{(ph)}\\ \eta_{(ph)}\\ \eta'_{(ph)}\\ K^0_{(ph)} \\ \bar K^0_{(ph)}\\ a_{(ph)}-\langle a \rangle\end{pmatrix} = \begin{pmatrix}1 & -\theta_{\pi^0\eta} & -\theta_{\pi^0 \eta'} & 0 & 0 & \epsilon_a \theta_{\pi^0 a}\\ \theta_{\pi^0\eta} & 1 & 0 & 0 & 0 & \epsilon_a \theta_{\eta a}\\ \theta_{\pi^0\eta'} & 0 & 1 & 0 & 0 & \epsilon_a \theta_{\eta' a}\\ 0 & 0 & 0 & 1 & 0 & \epsilon_a\theta_{K^0 a}\\ 0 & 0 & 0 & 0 & 1 & \epsilon_a \theta_{\bar K^0 a}\\ \epsilon_a \theta_{a \pi^0} & \epsilon_a \theta_{a\eta} & \epsilon_a \theta_{a\eta'} & \epsilon_a \theta_{a K^0} & \epsilon_a \theta_{a \bar K^0} & 1 + \epsilon_a^2 \theta_{aa}\end{pmatrix} \begin{pmatrix}\pi^0\\ c_\eta \eta_8 - s_\eta \eta_0\\ s_\eta \eta_8 + c_\eta \eta_0\\ K^0 \\ \bar K^0 \\ a\end{pmatrix} $$


$$\begin{align}
\theta_{\pi^0 a} + \theta_{a \pi^0} + \theta_{\pi^0\eta}\theta_{\eta a} + \theta_{\pi^0 \eta'}\theta_{\eta' a} &= \frac{1}{2} (\bar c_{uu}^A -\bar c_{dd}^A )\\
c_\eta (\theta_{\eta a} + \theta_{a \eta}-\theta_{\pi^0\eta}\theta_{\eta a}) + s_\eta (\theta_{\eta' a}+\theta_{a\eta'}-\theta_{\pi^0 \eta'}\theta_{\eta' a})&= \frac{1}{2\sqrt{3}}(\bar{c}_{uu}^A +\bar c_{dd}^A -2 \bar c_{ss}^A)  \\
-s_\eta (\theta_{\eta a} + \theta_{a \eta}-\theta_{\pi^0\eta}\theta_{\eta a}) + c_\eta (\theta_{\eta' a}+\theta_{a\eta'}-\theta_{\pi^0 \eta'}\theta_{\eta' a})&= \frac{1}{\sqrt{6}}(\bar{c}_{uu}^A +\bar c_{dd}^A + \bar c_{ss}^A)  \\
\theta_{\bar K^0 a} + \theta_{a K^0} &= \frac{1}{\sqrt{2}}\bar c_{sd}^A\\
\theta_{K^0 a} + \theta_{a \bar K^0} &= \frac{1}{\sqrt{2}}\bar c_{ds}^A\\
\theta_{\pi^0 a}^2 + \theta_{\eta a}^2 + \theta_{\eta' a}^2 + 2 \theta_{K^0 a}\theta_{\bar K^0 a} + 2\theta_{aa} &= \frac{1}{2}[(\bar c_{uu}^A)^2 + (\bar c_{dd}^A)^2 + (\bar c_{ss}^A)^2 + 2 \bar c_{ds}^A \bar c_{sd}^A] \\
-m_a^2 \theta_{a\pi^0}\frac{\langle a\rangle}{f_a} &=\frac{1}{2} \left[\sin(\alpha_u - 2\varphi_{uu})(m_{\bar K}^2 - \Delta^2 + \epsilon_I) - c_{u_0}^2\sin(\alpha_d - 2\varphi_{dd}) (m_{\bar K}^2 -\Delta^2 -\epsilon_I) + s_{u_0}^2\sin(\alpha_s - \varphi_{dd}-\varphi_{ss})(m_{\bar K}^2 + \Delta^2) \right]\\
-m_a^2 (c_\eta \theta_{a\eta} + s_\eta \theta_{a\eta'})\frac{\langle a\rangle}{f_a}&= \frac{1}{2\sqrt{3}} \left[\sin(\alpha_u - 2\varphi_{uu})(m_{\bar K}^2 -\Delta^2 + \epsilon_I) + c_{u_0}^2 \sin(\alpha_d - 2\varphi_{dd})(m_{\bar K}^2-\Delta^2-\epsilon_I) -2c_{u_0}^2\sin(\alpha_s - 2\varphi_{ss})(m_{\bar K}^2 + \Delta^2)+2s_{u_0}^2 \sin(\alpha_d-\varphi_{dd}-\varphi_{ss})(m_{\bar K}^2-\Delta^2-\epsilon_I) - s_{u_0}^2 \sin(\alpha_s-\varphi_{dd}-\varphi_{ss})(m_{\bar K}^2 + \Delta^2)\right]\\
-m_a^2(s_\eta \theta_{a\eta}-c_\eta \theta_{a\eta'})\frac{\langle a \rangle}{f_a}&= -\frac{m_0^2}{\sqrt{6}}(\theta_0 + 2\varphi_{uu}+2\varphi_{dd} + 2\varphi_{ss}) +\frac{1}{\sqrt{6}}\left[\sin(\alpha_u - 2\varphi_{uu})(m_{\bar K}^2 -\Delta^2 + \epsilon_I) + c_{u_0}^2 \sin(\alpha_d - 2\varphi_{dd})(m_{\bar K}^2-\Delta^2-\epsilon_I) +c_{u_0}^2\sin(\alpha_s - 2\varphi_{ss})(m_{\bar K}^2 + \Delta^2)-s_{u_0}^2 \sin(\alpha_d-\varphi_{dd}-\varphi_{ss})(m_{\bar K}^2-\Delta^2-\epsilon_I) - s_{u_0}^2 \sin(\alpha_s-\varphi_{dd}-\varphi_{ss})(m_{\bar K}^2 + \Delta^2)\right]\\
- m_a^2 \theta_{a K^0}\frac{\langle a\rangle}{f_a} &= \frac{i}{\sqrt{2}}s_{u_0} c_{u_0}\left[\cos(\alpha_d - 3 \varphi_{dd}/2-\varphi_{ss}/2)(m_{\bar K}^2-\Delta^2-\epsilon_I) + \cos(\alpha_s - \varphi_{dd}/2 -3\varphi_{ss}/2)(m_{\bar K}^2 +\Delta^2)\right] e^{i \Delta_{sd}/2}\\
- m_a^2 \theta_{a \bar K^0}\frac{\langle a\rangle}{f_a} &= - \frac{i}{\sqrt{2}}s_{u_0} c_{u_0}\left[\cos(\alpha_d - 3 \varphi_{dd}/2-\varphi_{ss}/2)(m_{\bar K}^2-\Delta^2-\epsilon_I) + \cos(\alpha_s - \varphi_{dd}/2 -3\varphi_{ss}/2)(m_{\bar K}^2 +\Delta^2)\right] e^{-i \Delta_{sd}/2}\\
- m_a^2 \frac{\langle a\rangle}{f_a} &=  \frac{c_G F_0^2 m_0^2}{3 f_a^2}(\theta_0 + 2\varphi_{uu}+2\varphi_{dd} + 2\varphi_{ss}) 
\end{align}$$

Combining the last two equations, we can conclude that $s_{u_0} \sim \frac{F_0^2}{f_a^2}\approx 0$, $c_{u_0}\approx 1$
# Footnotes

[^1]: [[Axion-meson mixing in light of recent lattice $η$-$η'$ simulations and their two-photon couplings within $U(3)$ chiral theory (2211.02867v2)]]

[^2]:  To compare with their results, set $c_G=-1/2$, $c^A_u=c^A_d=c^A_s = 0$