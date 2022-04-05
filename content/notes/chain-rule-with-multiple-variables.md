---
title: Chain rule with multiple variables
disableToc: true
---

### Chain rule with multiple variables
When applying the [[chain rule]] to [[notes/multivariable-functions|functions with multiple]] variables, we must keep in mind that each of our internal functions can have several variables as well.

**Case 1:**
$z = f(x,y)$ with $x=g(t)$ and $y=h(t)$. The function can be rewritten as $z=f(g(t),h(t))=F(t)$, since $x$ and $y$ share the same internal variable.

$$
\frac{dz}{dt}=\frac{\partial z}{\partial x}\frac{dx}{dt}+\frac{\partial z}{\partial y}\frac{dy}{dt}
$$
#math #calculus 
