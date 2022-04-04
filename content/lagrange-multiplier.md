---
title: "Lagrange Multiplier"
disableToc: true
---

### Lagrange Multiplier
Given a [multivariable function](multivariable-functions.md), and a [constraint](constrained-maximum-minimum.md), we use a Lagrange Multiplier, $\lambda$, to find its minimums and maximums. The Lagrangian Function has the form:
$$
\mathcal{L}(x,\lambda)=f(x)-\lambda g(x)
$$
Where $f(x)$ is the original function and $g(x)$ is the constraint. This can be generalized for any number of variables.

##### Example
We'll use the same example as in the [constraint](constrained-maximum-minimum.md) note.

Given a function $w=x^2+y^2+z^2$, we have the constraint $2z+x-y=6$. Find the critical points of the original function and whether they're maximums, minimums, or saddle points.

We'll rewrite the functions as a Lagrangian function.

$$
\begin{align}
	\mathcal{L}(x,y,z,\lambda)&=f(x,y,z)-\lambda g(x,y,z) \\
	\mathcal{L}(x,y,z,\lambda)&=(x^2+y^2+z^2)-\lambda(x-y+2z-6) \\
	\mathcal{L}(x,y,z,\lambda)&=x^2+y^2+z^2-\lambda x+\lambda y-2\lambda z+6 \lambda
\end{align}
$$

With this new function $\mathcal{L}$, we now find the partial derivatives for each variable and equalize them to $0$.


$$\begin{align}
	\mathcal{L}_x&=2x-\lambda=0 \\
	\mathcal{L}_y&=2y+\lambda=0 \\
	\mathcal{L}_z&=2z-2\lambda=0 \\
	\mathcal{L}_\lambda &=-x+y-2z+6=0 \\
\end{align}$$


This gives us a system of equations, and we can solve for $x,y,z$, giving us the coordinates for our critical point.
$$
\begin{align}
	x=1\\
	y=-1\\
	z=2\\
	\lambda=2
\end{align}
$$
#### Multiple Constraints
The Lagrange Multiplier can be applied to problems with multiple constraints, with the function:
$$
\mathcal{L}(x,\lambda_1,\lambda_2,\dots,\lambda_n)=f(x)-\lambda_1g_1(x)-\lambda_2g_2(x)-\dots-\lambda_ng_n(x)
$$
##### Example
Given the function $f(x,y,z)=xy+yz$, and the constraints $g_1(x,y)=x^2+y^2=8$, $g_2(y,z)=yz=8$, find the extrema using Lagrange Multiplication.
![solution](2022-04-04-122210_1158x751_scrot.png)

#math #calculus 
