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

##### Example
Evaluate $F=zi+xj+yk$, applied on the curve of the cylinder $x^2+y^2=1$ in the plane $y+z=2$. The curve is oriented clockwise when seen from above.

Rotating the force vector gives us:
$$
\text{rot}\vec{F}=[i+j+k]
$$
Now we find the normal vector, taking $y+z=2$ as the plane equation.
$$
\begin{align}
	n=\frac{\nabla h}{\nabla|h|} \\\\
	h=y+z-2=0 \\\\
	n = \frac{j+k}{\sqrt{j^2+k^2}}
\end{align}
$$
Since all our vectors are canonical vectors, this becomes:
$$
\begin{align}
	i^2=j^2=k^2=1 \\\\
	n =\frac{j+k}{\sqrt{2}}
\end{align}
$$
