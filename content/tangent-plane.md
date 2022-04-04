---
title: Tangent Plane
disableToc: true
---

### Tangent Plane
The infinitely small point on $z=f(x,y)$ is flat, and if we were to extend it infinitely across [3 dimensions](coordinate-systems-in-3-dimensions.md), we'll get a tangent plane to the original surface.

The plane tangent to the surface $z=f(x,y)$ at the point $P=(x_0,y_0,z_0)$ is:
$$
z-z_0=f_x(x_0,y_0)(x-x_0)+f_y(x_0,y_0)(y-y_0)
$$

##### Example
Find the equation of the plane tangent to $z=2x^2+y^2$ at the point $P(1,1,3)$.

First we find the partial derivatives with respect to $x$ and $y$.
$$
\begin{align}
	f_x(x_0, y_0) = 4x && f_x(1,1)=4 \\
	\\
	f_y(x_0, y_0) = 2y && f_y(1,1)=2 \\
\end{align}
$$
$$
\begin{align}
	z-3&=4(x-1)+2(y-1) \\
	z &= 4x+2y+3 \\
\end{align}
$$

#math #calculus 
