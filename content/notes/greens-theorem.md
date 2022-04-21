---
title: "Green's Theorem"
disableToc: true
---

### Green's Theorem
Supposing that $C$ is a simple closed curve over a range $R$. If $P$ and $Q$, being vectorial functions, and their derivatives are continuous over $R$, then:
$$
\oint_C P(x,y)dx+Q(x,y)dy=\iint_R \frac{\partial Q}{\partial x}-\frac{\partial P}{\partial y}dA
$$

#### Proof
Considering a curve $C$ subjected to a simple vector field $P(x,y)$
$$
\oint_CP\mathrm{d}x=\int_{a}^{b} \mathrm{d}x+\int_{b}^{a} P\mathrm{d}x=
\int_{a}^{b} P(x_1,y)\mathrm{d}x-\int_{a}^{b} P(x_2,y)\mathrm{d}x=
\int_{a}^{b} P(x,y) |_{x_1}^{x_2}=
$$

$$
\int_{a}^{b} \int_{x_2}^{x_1} \frac{\partial P}{\partial y}\mathrm{d}y\mathrm{d}x=
-\int_{a}^{b} \int_{x_2}^{x_1} \frac{\partial P}{\partial y}\mathrm{d}A
$$



![[files/2022-04-20-085721_729x835_scrot.png]]
#math