---
title: Linear Transformations
disableToc: true
---

### Linear Transformations
The linear transformation $T: \mathbb{R}^n \to \mathbb{R}^m$, where $n$ and $m$ can be $2,3$, is a function that has the following properties:
1. $T(x+y) = T(x)+T(y), x,y \in \mathbb{R}^n$
2. $T(ax)=aT(x), a \in \mathbb{R}, x \in \mathbb{R}^n$

This first property shows that applying a transformation to a sum of vectors is the same applying the transformation to the [[notes/vector|vectors]] and then adding the results.
The second property shows that scalar multiplication in transformations is distributive.

Linear transformations can also be applied to $n \times m$ [[notes/matrix|matrices]], depending on the dimensional space.

##### Example
Let $T: \mathbb{R}^2 \to \mathbb{R}^2$ be defined as $T(v_1,v_2) = (v_1-v_2, v_1+2v_2)$. Check if $T$ is a linear transformation.
$$
\begin{align}
	T: \mathbb{R}^2 &\longrightarrow \mathbb{R}^2 \\
	\begin{bmatrix}
		v_1 \\
		v_2 \\
	\end{bmatrix} &\longmapsto
	\begin{bmatrix}
		v_1-v_2 \\
		v_1+2v_2
	\end{bmatrix}
\end{align}
$$
First, we'll check for the first property. We can assign general variables instead of specific numbers.
$$
\begin{align}
	\vec{x}=
	\begin{bmatrix}
		\alpha \\
		\beta \\
	\end{bmatrix} &&
	\vec{y}=
	\begin{bmatrix}
		\gamma \\
		\zeta \\
	\end{bmatrix} &&
	\alpha, \beta, \gamma, \zeta \in \mathbb{R} \\
\end{align}
$$
Now we see the result of $T(\vec{x}+\vec{y})$
$$
\begin{align}
	\vec{x}+\vec{y}=
	\begin{bmatrix}
		\alpha + \gamma \\
		\beta + \zeta \\
	\end{bmatrix} \\ \\
	T(\vec{x}+\vec{y})=
	\begin{bmatrix}
		(\alpha + \gamma) - (\beta + \zeta) \\
		(\alpha + \gamma) + 2(\beta + \zeta) \\
\end{bmatrix}
\end{align}
$$
We compare this to the result of $T(\vec{x}) + T(\vec{y})$
$$
\begin{align}
	T(\vec{x})=
	\begin{bmatrix}
		\alpha-\beta \\
		\alpha + 2\beta \\
	\end{bmatrix} \\ \\
	T(\vec{y})=
	\begin{bmatrix}
		\gamma - \zeta \\
		\gamma + 2\zeta \\
	\end{bmatrix} \\ \\
	T(\vec{x})+T(\vec{y})=
	\begin{bmatrix}
		(\alpha - \beta) + (\gamma - \zeta) \\
		(\alpha + 2\beta) + (\gamma + 2\zeta) \\
	\end{bmatrix}
\end{align}
$$
The result of both of these sums is equal, which proves the first property.

To prove the second property, we can multiply some vector $x$ by a scalar $alpha$
$$
\begin{align}
	\vec{x}=
	\begin{bmatrix}
		a \\
		b
	\end{bmatrix} &&
	\alpha \in \mathbb{R}, a \land b \in \mathbb{R}^2
\end{align}
$$
First we'll find the result of $\alpha T(\vec{x})$:
$$
\begin{align}
	T(\vec{x})=
	\begin{bmatrix}
		a - b \\
		a + 2b \\
	\end{bmatrix} \\ \\
	\alpha T(\vec{x})=\alpha
	\begin{bmatrix}
		a - b \\
		a + 2b \\
	\end{bmatrix}=
	\begin{bmatrix}
		\alpha(a-b) \\
		\alpha(a+2b) \\
	\end{bmatrix}
\end{align}
$$
Now we see the result of $T(\alpha \vec{x})$
$$
\begin{align}
	\alpha \vec{x}=
	\begin{bmatrix}
		\alpha a \\
		\alpha b \\
	\end{bmatrix} \\ \\
	T(\alpha \vec{x})=
	\begin{bmatrix}
		\alpha a - \alpha b \\
		\alpha a + 2\alpha b \\
	\end{bmatrix}
\end{align}
$$
Looking at the resultes of these transformations, we can see that they're the same, fulfilling the second property. Since this transformation fulfills both properties, this transformation is linear.

#math #linearAlgebra 
