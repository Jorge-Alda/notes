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

According to Srednicki, eq.(94.18), the full pseudoscalar matrix is
$$\boldsymbol{U} = \sqrt{\boldsymbol{U_0}}\exp\left(\frac{i}{F_0}\boldsymbol{\lambda_a} \pi^a\right)\sqrt{\boldsymbol{U_0}}$$

# Mixing of pseudoscalar fields at LO

We follow the steps of[^1], but introducing the derivative coupling to quarks in addition to the anomalous couplings to gluons[^2].

## Diagonalization of the kinetic term

We define the fields $$\begin{pmatrix}\eta\\ \eta'\end{pmatrix}=\begin{pmatrix}c_\eta & -s_\eta\\ s_\eta & c_\eta\end{pmatrix}\begin{pmatrix}\eta_8\\\eta_0\end{pmatrix} $$ which are orthogonal at LO.

We denote the fields that diagonalize the kinetic term at LO by a $(K)$ subindex. The transformation is given by
$$\begin{pmatrix}\pi^0_{(K)}\\ \eta_{(K)}\\ \eta'_{(K)}\\ a_{(K)}\end{pmatrix} = \begin{pmatrix}1 & 0 & 0 & k_{a\pi^0}\\ 0 & 1 & 0 & k_{a\eta}\\ 0 & 0 & 1 & k_{a\eta'}\\k_{a\pi^0} & k_{a\eta} & k_{a\eta'} & 1\end{pmatrix} \begin{pmatrix}\pi^0\\ \eta\\ \eta'\\ a\end{pmatrix}$$

$$\begin{align}
k_{a\phi} &= \frac{F_0}{2f_a}\langle \boldsymbol{c_q^A}\boldsymbol{\lambda_\phi}\rangle\\
k_{a\pi^0} &=\frac{F_0}{4f_a}(c_u^A-c_d^A) \\
k_{a\eta} &= \frac{F_0}{4f_a}\left[\frac{c_\eta}{\sqrt{3}}(c_u^A + c_d^A -2c_s^A)-\frac{2s_\eta}{\sqrt{6}}(c_u^A+c_d^A+c_s^A)\right] \\
k_{a\eta'}  &= \frac{F_0}{4f_a}\left[\frac{s_\eta}{\sqrt{3}}(c_u^A + c_d^A -2c_s^A)+\frac{2c_\eta}{\sqrt{6}}(c_u^A+c_d^A+c_s^A)\right] 
\end{align}
$$


## Diagonalization of the mass term

We will use as hadronic inputs $m_{\bar{K}}^2$, $\Delta^2 = m_{\bar{K}}^2 - m_{\bar{\pi}}^2$ and $\epsilon_I = B_0 (m_u-m_d) = m_{K^+}^2 - m_{K^0}^2-(m_{\pi^+}^2-m_{\pi^0}^2)$. At LO, the quark masses are $$|\boldsymbol{m_q}|=\frac{1}{2B_0}\begin{pmatrix}m_{\bar{K}}^2-\Delta^2 + \epsilon_I & 0 & 0\\ 0 & m_{\bar{K}}^2-\Delta^2 - \epsilon_I & 0\\ 0 & 0 & m_{\bar{K}}^2+\Delta^2\end{pmatrix}$$
With this, the masses of the eta mesons and their mixing angle are 
$$\begin{align}
m_\eta^2 &= m_{\bar{K}}^2 + \frac{1}{2}m_0^2 - \frac{1}{2}\sqrt{m_0^4 -\frac{4}{3}m_0^2 \Delta^2 + 4\Delta^4}\\ 
m_{\eta'}^2 &= m_{\bar{K}}^2 + \frac{1}{2}m_0^2 + \frac{1}{2}\sqrt{m_0^4 -\frac{4}{3}m_0^2 \Delta^2 + 4\Delta^4}\\
\cos(2\theta_\eta) &= 2 c_\eta^2-1 = \frac{\frac{2}{3}\Delta^2-m_0^2}{\sqrt{m_0^4 -\frac{4}{3} m_0^2 \Delta^2 + 4\Delta^4}}
\end{align}$$

The mass terms, written with the Lagrangian fields, are
$$\mathcal{L}\supset-\frac{1}{2}m_\pi^2 {\pi^0}^2 -\frac{1}{2}m_\eta^2 \eta^2 - \frac{1}{2}m_{\eta'}^2 {\eta'}^2-\frac{1}{2}\left(\mu_a^2 +\frac{2}{3}c_G^2\frac{F_0^2}{f_a^2}m_0^2\right) a^2-M_{\pi^0\eta}^2 \pi^0 \eta -M_{\pi^0\eta'}^2 \pi^0 \eta' + \sqrt{\frac{2}{3}}m_0^2 c_G \frac{F_0}{f_a} (c_\eta \eta' - s_\eta \eta) a$$

$$\begin{pmatrix}\pi^0_{(M)}\\ \eta_{(M)}\\ \eta'_{(M)}\\ a_{(M)}\end{pmatrix} = \begin{pmatrix}1 & -\mu^2_{\pi^0\eta} & -\mu^2_{\pi^0\eta'} & -\mu^2_{\pi^0 a}\\ \mu^2_{\pi^0\eta} & 1 & 0 & -\mu^2_{\eta a}\\ \mu^2_{\pi^0\eta'} & 0 & 1 & -\mu^2_{a\eta'}\\\mu^2_{\pi^0 a} & \mu^2_{\eta a} & \mu^2_{\eta' a} & 1\end{pmatrix}\begin{pmatrix}\pi^0_{(K)}\\ \eta_{(K)}\\ \eta'_{(K)}\\ a_{(K)}\end{pmatrix} = \begin{pmatrix}1 & -\mu^2_{\pi^0\eta} & -\mu^2_{\pi^0 \eta'} & k_{a\pi^0}-\mu^2_{\pi^0 a}-k_{a\eta}\mu^2_{\pi^0\eta}-k_{a\eta'}\mu^2_{\pi^0\eta'}\\ \mu^2_{\pi^0\eta} & 1 & 0 & k_{a\eta} -\mu^2_{\eta a}+k_{a\pi^0}\mu^2_{\pi^0 \eta}\\ \mu^2_{\pi^0\eta'} & 0 & 1 &  k_{a\eta'} -\mu^2_{\eta' a}+k_{a\pi^0}\mu^2_{\pi^0 \eta'}\\ k_{a \pi^0} + \mu^2_{\pi^0 a} & k_{a\eta} + \mu^2_{\eta a} & k_{a\eta'}+\mu^2_{\eta' a} & 1 + k_{a\pi^0}\mu^2_{\pi^0 a} + k_{a\eta}\mu^2_{\eta a}+k_{a\eta'}\mu^2_{\eta' a}\end{pmatrix} \begin{pmatrix}\pi^0\\ \eta\\ \eta'\\ a\end{pmatrix} $$

$$\begin{align}
\mu^2_{\pi^0\eta} &= -\frac{\epsilon_I}{\sqrt{3}}\frac{c_\eta - \sqrt{2}s_\eta}{m_\pi^2 - m_\eta^2}\\
\mu^2_{\pi^0\eta'} &= -\frac{\epsilon_I}{\sqrt{3}}\frac{\sqrt{2}c_\eta+ s_\eta}{m_\pi^2 - m_{\eta'}^2}\\
0 &= -k_{a\pi^0}(\mu_a^2 +m_\pi^2) + \mu^2_{\pi^0 a}(\mu_a^2 - m_\pi^2) + k_{a\eta}\mu^2_{\pi\eta}(\mu_a^2 + m_\eta^2)+m_\eta^2 \mu^2_{\eta a}\mu^2_{\pi\eta} + k_{a\eta'}\mu^2_{\pi\eta'}(\mu_a^2 + m_{\eta'}^2)+m_{\eta'}^2 \mu^2_{\eta' a}\mu^2_{\pi\eta'} \\
-\sqrt{\frac{2}{3}}m_0^2 s_\eta c_G \frac{F_0}{f_a} &= - k_{a\eta}(\mu_a^2 +m_\eta^2) + \mu^2_{\eta a}(\mu_a^2 - m_\eta^2) - [k_{a\pi^0}\mu^2_{\pi^0\eta}(\mu_a^2 + m_\pi^2)+m_\pi^2 \mu^2_{\pi^0 a} \mu^2_{\pi^0\eta}]\\
\sqrt{\frac{2}{3}}m_0^2 c_\eta c_G \frac{F_0}{f_a} &= - k_{a\eta'}(\mu_a^2 +m_{\eta'}^2) + \mu^2_{\eta' a}(\mu_a^2 - m_{\eta'}^2) - [k_{a\pi^0}\mu^2_{\pi^0\eta'}(\mu_a^2 + m_\pi^2)+m_\pi^2 \mu^2_{\pi^0 a} \mu^2_{\pi^0\eta'}]\\
m_a^2 &= \mu_a^2(1 - 2k_{a\pi^0}\mu^2_{\pi^0 a} - 2k_{a\eta}\mu^2_{\eta a} -2k_{a\eta'}\mu^2_{\eta' a} ) + \frac{2}{3}c_G^2 \frac{F_0^2}{f_a^2}m_0^2 - m_\pi^2(k_{a\pi^0} + \mu^2_{\pi^0 a})^2 - m_\eta^2(k_{a\eta} + \mu^2_{\eta a})^2 - m_{\eta'}^2(k_{a\eta'} + \mu^2_{\eta' a})^2
\end{align}$$

QCD axion, i.e. $c_u =c_d =c_s = 0$, $\mu_a^2=0$, $c_G=-1/2$:
$$\begin{align}
\mu^2_{\eta a} &= -\frac{m_0^2}{\sqrt{6}m_\eta^2}s_\eta \frac{F_0}{f_a} \\
\mu^2_{\eta' a} &= \frac{m_0^2}{\sqrt{6}m_{\eta'}^2}s_\eta \frac{F_0}{f_a} \\
m_a^2 &= \frac{m_0^2}{6}\frac{F_0^2}{f_a^2}\left(1 - \frac{m_0^2 s_\eta^2}{m_\eta^2} - \frac{m_0^2 c_\eta^2}{m_{\eta'}^2}\right)
\end{align}$$ 

Agreeing with 2211.02867, and consequently reproducing the well-known QCD axion mass when plugging the correct hadronic inputs (see discusion there...)


# Footnotes

[^1]: [[Axion-meson mixing in light of recent lattice $η$-$η'$ simulations and their two-photon couplings within $U(3)$ chiral theory (2211.02867v2)]]

[^2]:  To compare with their results, set $c_G=-1/2$, $c^A_u=c^A_d=c^A_s = 0$