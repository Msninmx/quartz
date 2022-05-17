---
title: "Surface Integrals"
disableToc: true
---
### Surface Integrals
Surface integrals are ways to integrate surfaces. This is done by converting the function defining the surface, normally defined as $r$, into coordinates, $u$ and $v$.
$$  \iint_{S}f(x,y,z)\mathrm{d}S=\iint_{D}f(r(u,v))\left |\frac{\partial r}{\partial u}\times \frac{\partial r}{\partial v}\right |\mathrm{d}u\mathrm{d}v
$$
$\mathrm{d}S$ is the infinitesimally small change in volume of the surface integral, and is volume of the infinitesimally small cube with sides $|r_u,\times r_v|$, $\mathrm{d}u$, $\mathrm{d}v$.

Surfaces defined as $z=g(x,y)$ can be parameterized as:
$$
\begin{align}
x=x &&
y=y &&
z=g(x,y)
\end{align}
$$
letting the function $r$ be defined as:
$$
  r=r(x,y)=xi+yj+g(x,y)k
$$
$\mathrm{d}S$ can also be rewritten to these parametric terms, being:
$$
\sqrt{\left( \frac{\partial z}{\partial x} \right)^2 + \left( \frac{\partial z}{\partial y} \right)^2 + 1}\quad\mathrm{d}A
$$
This parametrization can happen to any of the variables, not only $x$ and $y$.