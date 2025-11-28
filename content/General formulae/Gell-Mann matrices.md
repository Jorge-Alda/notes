---
title: Gell-Mann matrices
draft: false
tags:
  -
---

$$\lambda_1 = \begin{pmatrix} 0 & 1 & 0 \\ 1 & 0 & 0 \\ 0 & 0 & 0 \end{pmatrix}$$ 
$$\lambda_2 = \begin{pmatrix} 0 & -i & 0 \\ i & 0 & 0 \\ 0 & 0 & 0 \end{pmatrix}$$ 
$$\lambda_3 = \begin{pmatrix} 1 & 0 & 0 \\ 0 & -1 & 0 \\ 0 & 0 & 0 \end{pmatrix}$$ 
$$\lambda_4 = \begin{pmatrix} 0 & 0 & 1 \\ 0 & 0 & 0 \\ 1 & 0 & 0 \end{pmatrix}$$ 
$$\lambda_5 = \begin{pmatrix} 0 & 0 & -i \\ 0 & 0 & 0 \\ i & 0 & 0 \end{pmatrix}$$ 
$$\lambda_6 = \begin{pmatrix} 0 & 0 & 0 \\ 0 & 0 & 1 \\ 0 & 1 & 0 \end{pmatrix}$$ 
$$\lambda_7 = \begin{pmatrix} 0 & 0 & 0 \\ 0 & 0 & -i \\ 0 & i & 0 \end{pmatrix}$$ 
$$\lambda_8 = \frac{1}{\sqrt{3}} \begin{pmatrix} 1 & 0 & 0 \\ 0 & 1 & 0 \\ 0 & 0 & -2 \end{pmatrix}$$
## Normalization
$$\mathrm{tr}(\lambda_i \lambda_j) = 2 \delta_{ij}$$

## Commutation

$$\left[ \lambda_a, \lambda_b \right] = 2 i \sum_c f_{abc} \lambda_c$$
$$\{ \lambda_a, \lambda_b \} = \frac{4}{3} \delta_{ab} I + 2 \sum_c d_{abc} \lambda_c$$

- $f_{abc} = -\frac{1}{4} i \operatorname{tr}(\lambda_a [ \lambda_b, \lambda_c ])$ (antisymmetric)
	- $f_{123} = 1 \ , \quad f_{147} = f_{165} = f_{246} = f_{257} = f_{345} = f_{376} = \frac{1}{2} \ , \quad f_{458} = f_{678} = \frac{\sqrt{3}}{2}$
- $d_{abc} = \frac{1}{4} \operatorname{tr}(\lambda_a \{ \lambda_b, \lambda_c \})$ (symmetric)
	- $d_{146}=d_{157}=-d_{247}=d_{256}=d_{344}=d_{355}=-d_{366}=-d_{377} = \frac{1}{2}\,,\qquad d_{123}=d_{228}=d_{338}=-d_{888}=\frac{1}{\sqrt{3}}\,,\qquad d_{448}=d_{558}=d_{668}=d_{778}=\frac{-1}{2\sqrt{3}}$

$$\lambda_a \lambda_b = \frac{2}{3}\delta_{ab} 1+(d_{abc}+if_{abc})\lambda_c$$