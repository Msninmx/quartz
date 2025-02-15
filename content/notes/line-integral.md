---
title: "Line Integral"
disableToc: true
---

### Line Integral
Line integrals are those where the function is [[notes/integration|integrated]] along a curve on a scalar field or [[vector-field|vector field]].

#### Scalar field form
$$
\int_C f(x,y)ds = \int_C f(\boldsymbol{r})ds=\int_a^b f(\boldsymbol{r}(t))|\boldsymbol{r'}(t)dt
$$
Where:
- $ds$ is the length along the curve defined as $$dS=\sqrt{(\frac{dx}{dt})^2+(\frac{dy}{dt})^2}dt$$

#### Vector field form
$$
\int_C \boldsymbol{F}\cdot d \boldsymbol{r}=\int_a^b \boldsymbol{F}\cdot \boldsymbol{r'}(t)dt
$$
Line integrals on a [[vector-field|vectorial field]] can be seen as the sum of all the vectors produced by applying the vector functions on every point delimited by the curve.

$\boldsymbol{F}$ is generally a function for force, whose values for $x$ and $y$ are substituted with the components of $r$, the position function.


##### Example
Evaluate the integral $\int_C (xydx+x^2dy)$ on the interval $-1 \leq t \leq 2$ where $C$ is defined as $x=t$, $y=t^3$.

First, we convert the integral to functions of $t$, using the definition given for $C$.
$$
\begin{align}
	x&=t\\
	y&=t^3\\\\
	\frac{dx}{dt}=1	&& dx=dt\\\\
	\frac{dy}{dt}=3t^2 && dy = 3t^2dt
\end{align}
$$
This gives us the integral
$$
\begin{align}
	\int_{-1}^2(t)(t^3)dt+t^2[3t^2dt] \\
	\int_{-1}^24t^4 \\
\end{align}
$$
We can now solve and evaluate the integral with respect to $t$
$$
\int_{-1}^24t^4=\frac{4t^5}{5} \Big|_{-1}^2 =\frac{4}{5}[(2^5)-(-1^5)]=\frac{132}{5}
$$

##### Example
Evaluate the integral $\int_Cxy^2dS$ on the integral $0 \leq t \leq \frac{\pi}{2}$ where $C$ is defined as $x=4\cos t$, $y=\sin t$.

Rewriting the integral with respect to $t$
$$
\begin{align}
	\frac{dx}{dt}&=-4\sin t \\\\
	\frac{dy}{dt}&=4\cos t \\\\
\end{align}
$$
$$
\begin{align}
\int_0^{\frac{\pi}{2}}[4\cos t][4\sin t]^2\sqrt{[-\sin t]^2 + [4\cos t]^2} dt \\\\
\int_0^{\frac{\pi}{2}}64\sin^2t \cos t \sqrt{16}=256\int_0^{\frac{\pi}{2}}\sin^2t \cos t dt
\end{align}
$$
Now we solve the integral
$$
256\int_0^{\frac{\pi}{2}}u^2du=256\frac{u^3}{3}\Big|_0^{\frac{\pi}{2}}=\frac{256}{3}\sin^3t \Big|_0^{\frac{\pi}{2}}=\frac{256}{3}[\sin^3\frac{\pi}{2}-\sin^30]=\frac{256}{3}
$$
