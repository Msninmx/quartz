---
title: "Flux"
disableToc: true
---
### Flux
Flux is the measurement of flow, and is calculated using the [[notes/surface-integrals|integral]]:
$$
\iint F\cdot \mathrm{d}S
$$
When dealing with a flow field of the form $F(x,y,z)=Pi+Qj+Rk$, in some region $z=g(x,y)$, this integral can be rewritten as:
$$
\iint\left( -P\frac{\partial g}{\partial x} - Q\frac{\partial g}{\partial y} + R \right) \mathrm{d}A
$$
where $\mathrm{d}A$ changes depending on the coordinate system used.

##### Example
$F(x,y,z)=yi+xj+zk$ represents a flow field. Determine the flux $F$ in the region $E$ between the paraboloid $z=1-x^2-y^2$ and the plane $z=0$.

Given the formulae above, we only need to substitute values.
$$
\begin{align}
z=g(x,y)&=1-x^2-y^2 \\\\
\frac{\partial g}{\partial x}=-2x &\qquad
\frac{\partial g}{\partial y}=-2y
\end{align}
$$
The values of $P$, $Q$, and $R$ are given to us by the flow field:
$$
\begin{align}
P&=y \\
Q&=x \\
R&=z
\end{align}
$$
Plugging in these values to the integral gives us:
$$
\iint \left( 2xy + 2xy +z \right) \mathrm{d}A
$$
We can substitute the value of $z$ with our parameterized function:
$$
\iint \left( 2xy + 2xy +1-x^2-y^2 \right) \mathrm{d}A
$$
In order to evaluate the integral, we must convert to [[notes/polar-coordinates|polar coordinates]].
$$
  \int_{0}^{2\pi} \int_{0}^{1} \left[ 4\left[ r\cos\theta  \right]\left[ r\sin\theta  \right] + 1-r^2 \right] r\mathrm{d}r\mathrm{d}\theta
$$
The limits are determined by finding the range of the radius $r$, and the angle that it forms around our shape, $2\pi$.

Evaluating the integral with respect to $r$ first gives us:
$$
  \int_{0}^{2\pi} \sin\theta \cos\theta \mathrm{d}\theta +\frac{1}{4}\int_{0}^{2\pi} \mathrm{d}\theta 
$$
Solving the integral:
$$
  \left. \frac{\left( \sin\theta  \right)^2 }{2} + \frac{1}{4}\theta \right|_{0}^{2\pi}=
  \frac{\pi}{2}
$$
