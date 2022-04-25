---
title: "Polar Coordinates"
disableToc: true
---
### Polar Coordinates
On a Cartesian Plane, a point can be can be represented with a length and and angle:
$$
P(r,\theta)
$$
$r$ is defined as the distance between the point and the origin, and $\theta$ is the angle formed between $r$ and the $x$ axis.

#### Conversion to rectangular coordinates
To change from polar coordinates to rectangular ones:
$$
x=r\cos\theta\qquad y=r\sin\theta
$$
To change from rectangular coordinates to polar:
$$
r^2=x^2+y^2\qquad \tan\theta=\frac{y}{x}, \quad x\neq0
$$
#### Conversion to rectangular functions
To convert a function that accepts rectangular coordinates $(x,y)$, to one that accepts polar coordinates $(r,\theta)$, the substitution is the same.

##### Example
Express $x^2=4y$ in polar coordinates
$$
\begin{align}
x^2&=4y \\
(r\cos\theta)^2&=4(r\sin\theta) \\
r^2\cos^2\theta&=4r\sin\theta \\
r&=4\frac{\sin\theta}{\cos^2\theta} \\
r&=4\sec\theta\sin\theta
\end{align}
$$

#### Use Cases
One use case of polar coordinates are in [[notes/double-integration|double integrals]], either when the limits have terms of the form $x^2+y^2$, or when the function has terms of the form $x^2+y^2, x^2, y^2$.

