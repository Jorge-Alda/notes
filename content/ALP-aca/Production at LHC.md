---
title: Production at LHC
draft: false
tags:
  - ALP
  - ALPaca
  - ALPaca/new
---
 We have to compute $\sigma(pp\to a X)$, with $X$ being any other particle. This was used in [^1]

## Electroweak production
$pp \to a W$ and $pp\to a Z$, formulas by Gabriele
$$
\hat{\sigma} (u_\alpha \bar{d}_\beta \to W^- \!a) = \frac{\alpha_{\text{em}}^3 |V_{\alpha \beta}|^2}{1152\pi^2 f_a^2 s_W^2} |c_{WW}^{\text{eff}}|^2 \frac{\left(m_a^4+(\hat{s}-m_W^2)^2-2m_a^2(\hat{s}+m_W^2)\right)^{3/2}}{\hat{s}(\hat{s}-m_W^2)^2}\,,
$$

$$
\hat{\sigma} (q \bar{q}  \to Z \!a) = \frac{\alpha_{\text{em}}^3}{72\pi^2 f_a^2 s_W^2} (|A|^2+|B|^2) \frac{\left(m_a^4+(\hat{s}-m_Z^2)^2-2m_a^2(\hat{s}+m_Z^2)\right)^{3/2}}{\hat{s}^3}\,,
$$

$$    A= \frac{g_V^q\,c_{Z Z}^{\text{eff}}}{c_W} \frac{\hat{s}}{\hat{s}-m_Z^2} + \frac{1}{2}s_W\,Q_q c_{\gamma Z}^{\text{eff}}\,,\quad\quad B = \frac{g_A^q\,c_{Z Z}^{\text{eff}}}{c_W}\frac{\hat{s}}{\hat{s}-m_Z^2}\,,$$

$$   {\sigma}(p p\to V a)=  \sum_{k,l} \int \dfrac{\mathrm{d}\hat{s}}{s} \mathcal{L}_{q_k \bar q_l}\, \hat{\sigma}(q_k \bar q_l\to V a)  \,,$$

$$\mathcal{L}_{ q_k \bar  q_l}(\hat{s}) \equiv \int_{\hat{s}/s}^1 \dfrac{\mathrm{d}x}{x} \Big{[} f_{{q}_k} (x,\mu_F) f_{\bar{q}_l} (\frac{\hat{s}}{s x},\mu_F)+({q}_k \leftrightarrow \bar q_l)\Big{]}\,,$$

using the PDF set NNPDF23\_nlo\_as\_0119
- why PDF23? The most recent sets are PDF40
- Is the value of $\alpha_s(M_Z)$ important? This PDF uses $\alpha_s(M_Z) = 0.119$, but other values are available
- The output of the libraries is actually $x f(x;Q)$. Are we sure that the formulas are indeed correct?
- What is the factorization scale $\mu_F$?


## Gluon fusion, quark fusion
$\sigma(gg\to a)$  and $\sigma(q\bar q\to a)$ should be easy to compute. Is this the dominant channel?[^2]


## Production associated to jets
$pp \to a j$

For $c_G$ only, [^3]

## Bibliography

[^1]: [[Search for resonances decaying to photon pairs with masses between 4.9 and 19.4 GeV (2507.14390v1)]]

[^2]: [[Axion-Like Particles at Future Colliders (1808.10323v2)]]

[^3]: [[Probing axion-like particles coupling to gluons at the LHC (2203.01734v2)]]
