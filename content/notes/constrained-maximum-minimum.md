---
title: "Maximum and Minimum with Constrains"
disableToc: true
---

### Maximum and Minimum with Constraints
When solving problems involving [minimums and maximums](maximum-minimum.md), one can apply a constraint to the function.

##### Example
Given a function $w=x^2+y^2+z^2$, we have the constraint $2z+x-y=6$. Find the critical points of the original function and whether they're maximums, minimums, or saddle points.

For convention's sake, we assign $f(x,y,z)$ to the first function and $g(x,y,z)$ to the second function.

We equal $g$ to be zero, and solve for any of it's variables. For this example, we'll solve for $x$.
$$
\begin{align}
	g(x,y,z)=2z+x-y-6=0 \\
	x =y-2z+6
\end{align}
$$
We then substitute $x$ into $f$.
$$
\begin{align}
	w=x^2+y^2+z^2 \\
	w =(y-2z+6)^2+y^2+z^2
\end{align}
$$
Now that we have $f$ expressed as two variables, we can find its critical points.
$$
\begin{align}
	\frac{\partial w}{\partial y}&=4y-4z+12=0 \\
	\frac{\partial w}{\partial z}&=-4y+10z-24=0 \\
\end{align}
$$
$$
\begin{align}
\begin{cases}
	4y-4z+12=0 \\
	-4y+10z-24=0 
\end{cases} &&
y=-1 \quad z=2
\end{align}
$$
Substituting these values into our equation for $x$, we have our critical points( in this example only $1$).
$$
\text{Critical Point}=(1,-1,2)
$$
Now we find the determinant, to see if the critical point is a maximum, minimum, or saddle point.
$$
\begin{align}
	\frac{\partial^2w}{\partial y^2}&=4\\
	\frac{\partial^2w}{\partial z^2}&=10\\
	\frac{\partial^2w}{\partial z \partial y}&=-4\\
	D=4(10)&-(-4)^2=24
\end{align}
$$
Our determinant is positive, and so is $f_{xx}(-1,2)$, so the critical point is a minimum.

#math #calculus 