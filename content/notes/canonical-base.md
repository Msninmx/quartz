---
title: Canonical Base
disableToc: true
---
### Canonical Base

Canonical base in $\mathbb{R}^2$:
$$
\begin{align}
	e_i=
	\begin{bmatrix}
		1 \\ 0
	\end{bmatrix} &&
	e_2=
	\begin{bmatrix}
		0 \\ 1
	\end{bmatrix} &&
	\longrightarrow &&
	\begin{bmatrix}
		e_1 & e_2
	\end{bmatrix}=
	\begin{bmatrix}
		1 & 0 \\ 0 & 1
	\end{bmatrix}
\end{align}
$$


If we know the effects of a transformation on $e_1$ and $e_2$, in this example in $\mathbb{R}^2$, we can find the results of the transformation on any appropriate vector _without_ needing to know the transformation.
$$
T
\begin{bmatrix}
	x \\ y
\end{bmatrix}
=xT(e_1)+yT(e_2)
$$
This is due to the linearity of these transformations. With this, we can find our specific transformation. One way of doing this is finding the Matrix associated with our transformation.
$$
A_T=
\begin{bmatrix}
	T(e_1) & T(e_2)
\end{bmatrix}
$$
This will give us the transformation.
$$
\therefore T
\begin{bmatrix}
	x \\ y
\end{bmatrix}=
A_T
\begin{bmatrix}
	x \\ y
\end{bmatrix}
$$

