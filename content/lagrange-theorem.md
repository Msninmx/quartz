---
title: "Lagrange's Theorem"
disableToc: true
---

### Lagrange's Theorem
Lagrange's theorem states that if a function$f$ has a extrema at $x_0,y_0$, given the restriction $g$, then there exists some value $\lambda$ such that
$$
\nabla f(x_0,y_0)=\lambda \cdot \nabla g(x_0,y_0)
$$

where $\nabla$ is the [gradient vector](gradient-vector.md) of the function.
##### Example
At what point in the circle $x^2+y^2=1$ is the product $xy$ largest?

For this problem, we want to maximize the function $f(x,y)=xy$ given the constraint $g(x,y)=x^2+y^2-1=0$.

First we find the gradient vectors of our two functions.
$$
\begin{align}
	\nabla f(x,y)&=\langle y,x \rangle \\
	\nabla g(x,y)&=\langle 2x,2y \rangle \\
\end{align}
$$
We then use these vectors to simplify Lagrange's Theorem.
$$
\begin{align}
	\langle y,x \rangle = \lambda \cdot \langle2x,2y \rangle \\
	\langle y,x \rangle = \langle \lambda2x,\lambda2y \rangle \\\\
\end{align}
$$
This gives us a system of equations that we can solve, the two equations generated from Lagrange's Theorem, and our constraint equation.
$$
x=\pm\frac{1}{\sqrt{2}}\quad
y=\pm\frac{1}{\sqrt{2}}\quad
\begin{cases}
	y=\lambda2x \\
	x=\lambda2y \\
	x^2+y^2=1
\end{cases}\quad
$$
These values for $x$ and $y$ are extrema of our function $f$. We then evaluate the function with these values to check if they're maximums or minimums.
$$
\begin{align}
	f(\frac{1}{2},\frac{1}{2})&=\frac{1}{4} \\\\
	f(\frac{1}{2},-\frac{1}{2})&=-\frac{1}{4} \\\\
	f(-\frac{1}{2},\frac{1}{2})&=-\frac{1}{4} \\\\
	f(-\frac{1}{2},-\frac{1}{2})&=\frac{1}{4} \\\\
\end{align}
$$
Since the function returns the highest values for our first and fourth case, these are our maxima.

#math #calculus 