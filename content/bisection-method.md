---
title: "Bisection Method"
disableToc: true
---

### Bisection Method
This method looks to find the roots of a nonlinear equation.
1. First we find the range $[a,b]$ over which we want to check for roots.
2. We find the midpoint $m=\frac{a+b}{2}$ and evaluate $f(m)$.
3. If $f(m)=0$, then $m$ is our root.
4. If $f(a)$ and $f(m)$ have different signs, then the root is in the interval $[a,m]$.
5. If $f(b)$ and $f(m)$ have different signs, then the root is in the interval $[m,b]$.
6. We then divide this new interval in half and repeat the process.

This gives us an approximation for the root.

To find the accuracy of our approximation:
$$
\text{Error}=\frac{i_{current}-i_{previous}}{i_{current}}\times100
$$
Where $i$ is the value of the iteration. An acceptable error is around $1\times10^{-3}$

This method is useful for algebraic and transcendental equations, but is best used after a graphical analysis.

#### Intermediate Value Theorem
If $f(x)$ is constant over the range $[a,b]$, with $f(a)\cdot f(b)<0$, then there exists some value $c \in[a,b]$ where $f(c)=0$.

#math 