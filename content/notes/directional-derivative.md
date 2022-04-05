---
title: Directional Derivative
disableToc: true
---

### Directional Derivative
[[notes/partial-derivatives|Partial derivatives]] show us rates of change in $x$ and $y$ for a given function $f(x, y)$. Now we'll see rates of change on $f(x, y)$ in other directions, given by a vector $\vec{u}$.

There exists an infinite number of directions from where we can take the derivative. The point from where we take the derivative is $(x_0, y_0)$ and the distance is $\vec{u}$.

Directional derivatives in $\mathbb{R}^2$ have the form:
$$
D_uf(x_0,y_0)
$$
The unit [[notes/vector]] $\vec{u}$ shows the direction in which we create another axis $r$, giving us:
$$
D_\vec{u}f(x_0,y_0) = \frac{dz}{dr}
$$
The rate of change of $z$ with respect to $r$. $z$ is the function $f(x, y)$.

To find $dr$, we can apply trigonometric identities using $dx$ and $dy$.

We know how to find $dz$, the sum of the partial derivatives of $f(x,y)$. Therefore:

$$
D_\vec{u}f(x_0,y_0) = \frac{f_x(x_0,y_0)dx+f_y(x_0,y_0)dy}{dr}
$$

Which can be simplified as:
$$
D_\vec{u}f(x_0,y_0) = f_x(x_0,y_0)\frac{dx}{dr}+f_y(x_0,y_0)\frac{dy}{dr}
$$
We can substitute trigonometric functions to only need the angle of rotation:
$$
D_\vec{u}f(x_0,y_0) = f_x(x_0,y_0)\cos(\theta)+f_y(x_0,y_0)\sin(\theta)
$$
This process can be simplified even more finding the [[notes/gradient-vector|gradient vector]] of our function.
$$
D_\vec{u}f(x,y) = \langle f_x(x,y),f_y(x,y)\rangle \cdot \langle u_1, u_2 \rangle
$$
Dot product multiplies each element of one matrix with the corresponding element of the other matrix.

#math #calculus 
