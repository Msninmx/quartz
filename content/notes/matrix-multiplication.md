---
title: Matrix Multiplication
disableToc: true
---

### Matrix Multiplication
When multiplying a matrix by a scalar, each element of the matrix is multiplied by the constant.
$$
\begin{align}
	A=
	\begin{bmatrix}
		2 & 3 \\
		7 & 5\\
	\end{bmatrix} &&
	2A=
	\begin{bmatrix}
		4 & 6 \\
		14 & 10 \\
	\end{bmatrix}
\end{align}
$$

When multiplying matrices with each other, they must have the form $m \times p$ and $p \times n$. The resulting matrix will have the form $m \times n$, and each element will be found with the formula
$$
c_{ij}=\sum\limits_{k=1}^pa_{ik}b_{kj}
$$
The $j$ terms of our $a$ matrix increase until reaching $p$, and the same is done for the $i$ terms of the $b$ matrix.
##### Example
$$
\begin{align}
	D=
	\begin{bmatrix}
		5 & 6 & 7 \\
		0 & 1 & -2 \\
	\end{bmatrix} &&
	E=
	\begin{bmatrix}
		-1 & 0 \\
		4 & 5 \\
		7 & 9 \\
	\end{bmatrix}
\end{align}
$$
The matrices $D$ and $E$ are $2 \times 3$ and $3 \times 2$ respectively. Since the matrices have the same number on the "inside", in this case $3$, they are compatible. The final matrix will have a size of $2 \times 2$.
$$
DE=
\begin{bmatrix}
	5 & 6 & 7 \\
	0 & 1 & -2 \\
\end{bmatrix}
\begin{bmatrix}
	-1 & 0 \\
	4 & 5 \\
	7 & 9 \\
\end{bmatrix}
=
$$
First we take every number in the first row of our first matrix, and multiply it by its pair in the second matrix. Adding these results gives us the first element of our final matrix.
$$
\begin{align}
	5 \times -1 &= -5 \\
	6 \times 4 &= 24 \\
	7 \times 7 &= 49 \\
	\\
	-5 + 24 + 49 &= 68
\end{align}
$$
$$
\begin{bmatrix}
	68 &  \\
	 &  \\
\end{bmatrix}
$$
Repeating these steps for the rest of our rows and columns gives us the final matrix.
$$
DE=
\begin{bmatrix}
	68 & 93 \\
	-10 & -13 \\
\end{bmatrix}
$$
Matrix multiplication is not commutative; if we reverse the order of the matrices, we'll end up with one of size $3 \times 3$
$$
ED=
\begin{bmatrix}
	-5 & -6 & -7 \\
	20 & 29 & 18 \\
	35 & 51 & 31 \\
\end{bmatrix}
$$

#math #linearAlgebra #matrices 
