---
title: "Double Integration"
disableToc: true
---
### Double Integration
Double integration is the act of [[notes/integration|integrating]] some function several times. This can be done on a second [[notes/derivation|derivative]] of a single function, or the first [[notes/derivation|derivative]] of a [[notes/multivariable-functions|multivariable function]].
$$
\iint f(x,y)dxdy
$$
The order in which to integrate can be imagined as concentric circles going out; first the inside variables, in this example $dy$, then the outside circles, $dx$.

##### Example
We have the second derivative of some function $f$ as
$$
f_{xy}(xy)=2x+4xy
$$
Use a double integration to find each of the [[notes/partial-derivatives|partial derivatives]].
$$
\begin{align}
	\iint 2x+4xy\ dydy \\
	\int 2xdy+\int 4xydy \\
	2x\int dy + 4x\int ydy \\
	2xy + 2xy^2+C
\end{align}
$$
Here, we've integrated the function with respect to $y$. Now we integrate our result with respect to $x$. The $C$ can be ignored until we see differential equations, but it will be added at the end as the sum of all the constants.
$$
\begin{align}
	\int 2xy+2xy^2+Cdx \\
	2y\int xdx+2y^2\int xdx \\
	x^2y+x^2y^2+C
\end{align}
$$
This is the anti derivative of the function $f_{xy}(x,y)$.

This double integration can also be written as
$$
\int\left[\int 2x+4xy\ dy\right]dx
$$

#### Polar Coordinates
When evaluating a double integral, the limits of the integral can be functions, which in turn, means they can be functions using [[polar-coordinates|polar coordinates]].

#### Limits
Double integrals can also have limits, where each individual integration has it's own specific limits. If some of our limits are functions, they on the inside of the double integral.

If taking a double integral over some range $R$, the differential will be $dA$, which is the product of $dx\times dy$.
$$
\iint_Rf(x,y)dA
$$
When using polar coordinates, this is rewritten as:
$$
\iint_Rf(r\cos\theta,r\sin\theta)r\mathrm{d}r\mathrm{d}\theta
$$
##### Example
Let $R$ be the area between the circles $x^2+y^2=1$ and $x^2+y^2=5$.
Evaluate the integral
$$
\iint_R(x^2+y)\mathrm{d}A
$$
When dealing with problems involving circles, it's almost always best to work using [[polar-coordinates#Use Cases|polar coordinates]].

The problem gives us the radii of the two circles expressed as functions, which we can interpret as $r$ in polar coordinates. Since these limits are functions, they are the first limits in our integral.

![[2022-04-25-124817_733x749_scrot.png]]