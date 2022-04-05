---
title: Matrix of a System
disableToc: true
---

### Matrix of a System
Find the [[notes/matrix]] of the [[notes/linear-equation-systems|system]]:
$$
\begin{align}
	E_1:& 2x_1+3x_2-6x_3=9 \\
	E_2:& 4x_1+x_2+5x_3=13 \\
	E_1:& -2x_1+x_2+7x_3=2 \\
\end{align}
$$
$$
A=
\begin{bmatrix}
	2 & 3 & -8 \\
	4 & 1 & 5 \\
	-2 & 1 & 7 \\
\end{bmatrix}
$$
We take the coefficients of every term of our system of equations, and create a matrix with them.

The extended matrix is the right hand part of the equations:
$$
B=
\begin{bmatrix}
	9 \\
	13 \\
	2
\end{bmatrix}
$$
$$
(A|B)=
\left[
	\begin{array}{ccc|c}
		2 & 3 & -8 & 9 \\
		4 & 1 & 5 & 13 \\
		-2 & 1 & 7 & 2 \\
	\end{array}
\right]
$$
And our solution matrix:
$$
\vec{x}=
\begin{bmatrix}
	x_1 \\
	x_2 \\
	x_3 \\
\end{bmatrix}
$$
Giving us three matrices that represent our SLE.
$$A \vec{x}=B$$

#math #matrices #linearAlgebra 
