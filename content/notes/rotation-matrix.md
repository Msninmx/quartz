---
title: Rotation Matrix
disableToc: true
---

### Rotation Matrix
$$
A_\theta = 
\begin{bmatrix}
	\cos(\theta) & -\sin(\theta) \\
	\sin(\theta) & \cos(\theta) \\
\end{bmatrix}
$$
Multiplying this [[notes/matrix]] with a vector in $\mathbb{R}^2$ will rotate it.

##### Example
Let $\vec{v} = \begin{bmatrix} 2 \\ 1 \end{bmatrix}$, $\theta = \frac{\pi}{4}$
Rotate $\vec{v}$ by the angle $\theta$ counterclockwise.
$$
A_{\frac{\pi}{4}}=
\begin{bmatrix}
	\cos(\frac{\pi}{4}) & -\sin(\frac{\pi}{4}) \\
	\sin(\frac{\pi}{4}) & \cos(\frac{\pi}{4})
\end{bmatrix}
$$
$$
\vec{u}=
\begin{bmatrix}
	\frac{\sqrt{2}}{2} \\
	3 \frac{\sqrt{2}}{2}
\end{bmatrix}
$$
To prove this, we find the dot product of our vectors and divide it between the magnitudes. This should give us our angle $\frac{\pi}{4}$.

This type of transformation is similar to matrix [[notes/matrix-reflection|reflection]].

#math #matrices #linearAlgebra 
