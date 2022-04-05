---
title: Total Differential
disableToc: true
---

### Total Differential
Let $z=f(x,y)$ be a [[notes/multivariable-functions|multivariable function]] and $dx$ and $dy$ infinitely small changes in $x$ and $y$ respectively. How do we determine the total change in $z$?

Our total differential of our function $z$ is equal to the sum of the [[notes/partial-derivatives|partial differentials]] in $x$ and $y$.

The differential in $z$ is defined as:
$$
dz=f_x(x,y)dx+f_y(x,y)dy
$$

##### Example
Let $f(x)=\sqrt{x^2+y^2}$. Use the total differential to find the change in $f(x,y)$ when $(x,y)$ changes from $(3,4)$ to $(3.04, 3.98)$

We find the partial derivatives with respect of $x$ and $y$ of the function.
$$
df=\frac{x}{\sqrt{x^2+y^2}}dx + \frac{y}{\sqrt{x^2+y^2}}
$$
And we substitute our values of $x_0, y_0$, in this case $3, 4$, and our differential values, $0.04, -0.02$, for $dx, dy$
$$
df \approx\frac{3}{\sqrt{3^2+4^2}}(0.04)+\frac{4}{\sqrt{3^2+4^2}}(-0.02) \approx 0.008
$$
These equations are approximated since their composed of infinitely many tiny sums.

#math #calculus 
