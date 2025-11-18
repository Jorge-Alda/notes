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

$$V(a) = -F_0^2 [m_u \cos(\alpha_u-\varphi_u)+m_d \cos(\alpha_d-\varphi_d)+m_s \cos(\alpha_s-\varphi_s)]+\frac{m_0^2}{12}F_0^2\left[\theta_0-2\frac{c_G}{f_a}a + \varphi_u+\varphi_d+\varphi_s\right]^2+\frac{\mu_a^2}{2}a^2$$
The minimum of the ALP field is located at $$\langle a\rangle = \frac{c_G}{f_a}\frac{m_0^2 F_0^2}{3 m_a^2}(\theta_0 + \varphi_u + \varphi_d + \varphi_s)$$ where the physical mass is $$m_a^2 = \mu_a^2 +\frac{2}{3} c_G^2\frac{F_0^2}{f_a^2}m_0^2$$
 By shifting the ALP field from its minimum $a\to a - \langle a \rangle$,
 $$V =  -F_0^2 
 B_0 [m_u \cos(\alpha_u-\varphi_u)+m_d \cos(\alpha_d-\varphi_d)+m_s \cos(\alpha_s-\varphi_s)] -\frac{1}{2}m_a^2 a^2 +\frac{m_0^2}{12}F_0^2 \frac{\mu_a^2}{m_a^2}(\theta_0+\varphi_u + \varphi_d+\varphi_s)^2$$ $$B_0 m_u \sin(\alpha_u -\varphi_u) = B_0 m_d \sin(\alpha_d-\varphi_d) = B_0 m_s \sin(\alpha_s-\varphi_s)=\frac{m_0^2}{6}\frac{\mu_a^2}{m_a^2}(\theta_0+\varphi_u+\varphi_d+\varphi_s)$$ Note that if $\mu_a = 0$ (aka QCD axion), then $\varphi_i = \alpha_i$ irrespective of the value of $\theta_0$. For $\mu_a \neq 0$ and $\bar\theta$ small
 $$\varphi_i \approx \alpha_i - \frac{m_i^{-1}}{\mathrm{tr}(|\boldsymbol{m_q}|^{-1})+\frac{6B_0}{m_0^2}\frac{m_a^2}{\mu_a^2}}\bar{\theta}$$