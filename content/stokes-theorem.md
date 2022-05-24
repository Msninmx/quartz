---
title: "Stokes Theorem"
disableToc: true
---
### Stoke's Theorem
Stoke's theorem can be considered an extension of [[notes/greens-theorem|green's theorem]], and can be generalized to calculate the work done over a volume.

Let $F$ be a vector field. If the first derivatives are continuous along a space enclosing a surface $S$, then:
$$
  \oint_C(F\cdot T)\mathrm{d}s=\iint_{s}(rotF)\cdot n\mathrm{d}S
$$
Where $rotF$ is the rotation of the vector field, $n$ is a normal unit vector to $S$, and $\mathrm{d}S$ is equal to:
$$
\mathrm{d}S=
  \sqrt{1+\left( \frac{\partial z}{\partial x} \right)^2 + \left( \frac{\partial z}{\partial y} \right)^2 }
  \quad\mathrm{d}A
$$

