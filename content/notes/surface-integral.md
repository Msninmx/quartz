---
title: "Surface Integrals"
disableToc: true
---
### Surface Integrals
Similar to [[notes/line-integral|line integrals]], surface integrals take some function $f$ with $3$ variables, $x,y,z$.

This integral can be approximated as
$$
\mathrm{d}S=|r_u \times r_v| \mathrm{d}A
$$

Given this, we can have a parametric surface that can be integrated with
$$
  \iint_Sf(x,y,z)\mathrm{d}S=\iint_Df(r(u,v))|r_{u}\times r_{v}|\mathrm{d}A

$$

##### Example
Evaluate the integral $\iint_S \sqrt{1+x^2+y^2}\mathrm{d}S$, where $S$ is the surface defined by $r=u\cos vi + u\sin vj + vk$, where $0\leq u \leq 2$, $0\leq u \leq 4\pi$.

