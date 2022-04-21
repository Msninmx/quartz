---
title: "Volume and Double Integrals"
disableToc: true
---
### Volume and Double Integrals
We can use [[notes/double-integration|double integrals]] to find the volumes of solids.

If $f(x,y)\geq 0$, then the volume $V$ of the solid that is between the plane and below the surface $f$ is:
$$
V=\iint_Rf(x,y)dA
$$
where $R$ is the region being integrated, and  the differential of area $dA$, is equal to the product of the differential on $x$ and on $y$.

#### Case 1:
Volume over a closed rectangle:
$$
R=\{(x,y)\quad a\leq b\leq x; \quad c\leq y\leq d\}
$$

### Case 2:
Volume over a flat closed surface delimited by a function $g$:
$$
R=\{(x,y)\quad a\leq b\leq x; \quad g_1\leq y\leq g_2\}
$$
This is integrated as:
$$
\int_a^b\int_{y_1=g_1(x)}^{y_2=g_2(x)}f(x,y)dydx
$$
When integrating with limits defined by functions, we integrate with respect to these functions first.
 $x$ can also be 

#### Case 3:
