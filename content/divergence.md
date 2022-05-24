---
title: "Divergence"
disableToc: true
---
### Divergence
The divergence of a vector field gives us information about the [[flux]], and is calculated with:
$$
  divF=\nabla\cdot F=\frac{\partial F_{x}}{\partial x}\frac{\partial F_{y}}{\partial y}\frac{\partial F_{z}}{\partial z}
$$
#### Divergence Theorem
Let $D$ be a region enclosed by a smooth surface $S$ pointing upwards, and let $F$ be a vector field.

If the first partial derivatives are continuous over the space that contains S, then:
$$
  \oint_C(F\cdot n)\mathrm{d}S=\iiint_{D}(divF)\mathrm{d}V
$$

##### Example
Let $D$ be the region enclosed by the cube defined over $0\le x \le 1$,  $0\le y \le 1$,$0\le z \le 1$. Prove the divergence theorem over $F=xyi+y^2j+z^4k$.

First, we find the divergence of the flow field, by finding the partial derivatives of $F$:
$$
divF=y+2yz+3z^2
$$
So now we can establish our integral. The limits are given to us in the problem; the boundaries of the cube.
$$
  \int_{0}^{1} \int_{0}^{1} \int_{0}^{1} \left[ y+2yz+3z^2 \right] \mathrm{d}x\mathrm{d}y\mathrm{d}z
$$
Solving the integral gives us an answer of $2$.