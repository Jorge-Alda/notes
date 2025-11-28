---
title: Chiral Perturbation Theory
tags:
  - ChiPT
---
## The $SU(N_f)$ case

If we consider the symmetry breaking $SU(N_f)_L\times SU(N_f)_R  \to SU(N_f)_V$, there are $N_f^2-1$ light pseudoscalar pNGB's, for the $N_f=3$ case they are $(\pi, K, \eta)$.

Starting with the high-energy partonic Lagrangian

$$\mathcal{L} = -\frac{1}{4}G_{\mu\nu}^a G^{\mu\nu,a}+\bar{q}(i \cancel{D})q + \bar{q}\gamma^\mu (\boldsymbol{L}_\mu P_L + \boldsymbol{R}_\mu P_R)q -\bar{q}(\boldsymbol{S}-i\gamma_5\boldsymbol{P})q$$

This is matched to the low-energy $\chi$PT Lagrangian 

$$\mathcal{L}=\frac{F_0^2}{2}\langle D_\mu \boldsymbol{U} D^\mu\boldsymbol{U}^\dagger\rangle + \frac{F_0^2}{2}\langle \boldsymbol{\chi} \boldsymbol{U}^\dagger + \boldsymbol{\chi}^\dagger\boldsymbol{U}\rangle $$
- $F_0\approx f_\pi = 92\,\mathrm{MeV}$
- $$\boldsymbol{U}=\boldsymbol{U_0}\exp\left(\frac{i}{F_0}\begin{pmatrix}\pi^0 + \frac{\eta_8}{\sqrt{3}} & \sqrt{2} \pi^+ & \sqrt{2}K^+\\\sqrt{2}\pi^- & -\pi^0 +\frac{\eta_8}{\sqrt{3}} & \sqrt{2} K^0\\\sqrt{2}K^- & \sqrt{2}\bar{K}^0 & -\frac{2}{\sqrt{3}}\eta_8\end{pmatrix}\right)\equiv \boldsymbol{U_0}\exp\left(\frac{i}{F_0}\boldsymbol{\lambda_a} \pi^a\right)$$
- $\langle\cdots\rangle =\frac{1}{2}\mathrm{tr}(\cdots)$, $\langle \lambda_a \lambda_b^\dagger\rangle =\delta_{ab}$
- $$D_\mu\boldsymbol{U} = \partial_\mu\boldsymbol{U}-i\boldsymbol{R}_\mu \boldsymbol{U} + i \boldsymbol{U} \boldsymbol{L}_\mu$$
- $\boldsymbol{\chi} = 2 B_0 (\boldsymbol{S}+i\boldsymbol{P})$ with $B_0 = \frac{m_\pi^2}{m_u+m_d}$

Under *local* chiral rotations $(\boldsymbol{g_L}, \boldsymbol{g_R})\in SU(3)_L\times SU(3)_R$
- $\boldsymbol{U}\to \boldsymbol{g_R}\boldsymbol{U}\boldsymbol{g_L}^\dagger$
- $\boldsymbol{L}_\mu \to \boldsymbol{g_L}\boldsymbol{L}_\mu\boldsymbol{g_L}^\dagger+i \boldsymbol{g_L} \partial_\mu \boldsymbol{g_L}^\dagger$
- $\boldsymbol{R}_\mu \to \boldsymbol{g_R}\boldsymbol{R}_\mu\boldsymbol{g_R}^\dagger+i \boldsymbol{g_R} \partial_\mu \boldsymbol{g_R}^\dagger$
- $D_\mu\boldsymbol{U} \to \boldsymbol{g_R} D_\mu\boldsymbol{U}\boldsymbol{g_L}^\dagger$
- $\boldsymbol{\chi}\to\boldsymbol{g_R}\boldsymbol{\chi}\boldsymbol{g_L}^\dagger$
so the Lagrangian is invariant.

## $U(N_f)$

Due to the $U(1)_A$ anomaly, we also have to add a term accounting for the mass of the $\eta'$. This term is in fact related to the topological structure of the vacuum thanks to the Witten-Veneziano relation.

Adding the $\theta$ term to the high-energy Lagrangian
$$\mathcal{L} = -\frac{1}{4}G_{\mu\nu}^a G^{\mu\nu,a}+\bar{q}(i \cancel{D})q + \bar{q}\gamma^\mu (\boldsymbol{L}_\mu P_L + \boldsymbol{R}_\mu P_R)q -\bar{q}(\boldsymbol{S}-i\gamma_5\boldsymbol{P})q-\theta \frac{g_s^2}{32\pi^2}G_{\mu\nu}^a \tilde{G}^{\mu\nu,a}$$

The low-energy Lagrangian is now
$$\mathcal{L}=\frac{F_0^2}{2}\langle D_\mu \boldsymbol{U} D^\mu\boldsymbol{U}^\dagger\rangle + \frac{F_0^2}{2}\langle \boldsymbol{\chi} \boldsymbol{U}^\dagger + \boldsymbol{\chi}^\dagger\boldsymbol{U}\rangle -\alpha\frac{F_0^2}{4}\left[\theta-i\langle \log\boldsymbol{U} - \log\boldsymbol{U}^\dagger\rangle\right]^2$$ with Witten-Veneziano giving us $\alpha = \frac{m_0^2}{N_f}$

Now the Lagrangian is invariant under local chiral transformations $(\boldsymbol{g_L}, \boldsymbol{g_R})\in U(3)_L\times U(3)_R$, with (Srednicki, eq.(94.18))
- $$\boldsymbol{U}=\sqrt{\boldsymbol{U_0}}\exp\left(\frac{i}{F_0}\begin{pmatrix}\pi^0 + \frac{\eta_8}{\sqrt{3}}+\sqrt{\frac{2}{3}}\eta_0 & \sqrt{2} \pi^+ & \sqrt{2}K^+\\\sqrt{2}\pi^- & -\pi^0 +\frac{\eta_8}{\sqrt{3}}+\sqrt{\frac{2}{3}}\eta_0 & \sqrt{2} K^0\\\sqrt{2}K^- & \sqrt{2}\bar{K}^0 & -\frac{2}{\sqrt{3}}\eta_8+\sqrt{\frac{2}{3}}\eta_0\end{pmatrix}\right)\sqrt{\boldsymbol{U_0}}\equiv \sqrt{\boldsymbol{U_0}}\exp\left(\frac{i}{F_0}\boldsymbol{\lambda_a} \pi^a\right)\sqrt{\boldsymbol{U_0}}$$ $\langle \log\boldsymbol{U}\rangle = \frac{i}{F_0}\sqrt{\frac{3}{2}}\eta_0+\langle \log\boldsymbol{U_0}\rangle$
- $\theta \to \theta + i \log\det(\boldsymbol{g_R}\boldsymbol{g_L}^\dagger)$


### Complex quark masses

Let us assume that the quark have complex masses,
$$\mathcal{L}=-\bar{q} \boldsymbol{m_q} P_L q - \bar{q} \boldsymbol{m_q}^\dagger P_R q\,,\qquad \boldsymbol{m_q}=\mathrm{diag}(m_u e^{i\alpha_u}, m_d e^{i\alpha_d}, m_s e^{i\alpha_s})$$The matching to $\chi$PT is then
$$\boldsymbol{\chi} = 2 B_0 \boldsymbol{m_q}$$
Parametrizing the expectation value of the meson matrix as $\boldsymbol{U_0} =\mathrm{diag}(e^{i\varphi_u}, e^{i\varphi_d}, e^{i\varphi_s})$, the potential is
$$V = -F_0^2 B_0[m_u \cos(\alpha_u-\varphi_u)+m_d \cos(\alpha_d-\varphi_d)+m_s \cos(\alpha_s-\varphi_s)]+\frac{m_0^2}{12}F_0^2(\theta + \varphi_u+\varphi_d+\varphi_s)^2$$
The minimum of the potential is found for
$$B_0 m_u\sin(\alpha_u-\varphi_u)=B_0 m_d\sin(\alpha_d-\varphi_d) = B_0m_s\sin(\alpha_s-\varphi_s) = \frac{m_0^2}{6}(\theta+\varphi_u+\varphi_d+\varphi_s)$$ with the change of variables $\varphi'_i = \varphi_i-\alpha_i$ $$-B_0 m_u\sin(\varphi'_u)=-B_0 m_d\sin(\varphi'_d) = -B_0m_s\sin(\varphi'_s) = \frac{m_0^2}{6}(\bar\theta+\varphi'_u+\varphi'_d+\varphi'_s)$$
When CP is conserved, $\bar\theta = \theta + \alpha_u+\alpha_d+\alpha_s=0$, then the solution is particularly simple, $\varphi'_i=0 \Longrightarrow \varphi_i = \alpha_i$. If CP is not conserved but $\bar\theta$ is small,
$$\varphi_i \approx \alpha_i - \frac{m_i^{-1}}{\mathrm{tr}(|\boldsymbol{m_q}|^{-1})+\frac{6B_0}{m_0^2}}\bar{\theta}$$

## Neutron edm 

$$\boldsymbol{m_q}^\dagger\boldsymbol{U_0}\approx |\boldsymbol{m_q}|- \frac{i}{\mathrm{tr}(|\boldsymbol{m_q}|^{-1})+\frac{6B_0}{m_0^2}}\bar{\theta}\boldsymbol{1}\equiv |\boldsymbol{m_q}| - i \tilde{m} \bar{\theta}\boldsymbol{1}$$ ^e54958


Following Srednicki (eq 94.38), the edm of the neutron is $$d_n = \frac{e \bar{\theta} g_A c_+ \tilde{m}}{8\pi^2 f_\pi}\left[\log(\Lambda^2/m_\pi^2)+\mathcal{O}(1)\right]=3.2\times 10^{-16}\bar{\theta}\frac{\tilde{m}}{1.2\,\mathrm{MeV}} e\,\mathrm{cm}$$