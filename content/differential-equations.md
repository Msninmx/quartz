---
title: "Differential Equations"
disableToc: true
---
### Differential Equations
A differential equation is any equations that contains the derivative of one or more unknown functions.
$$
   a_n(x)\frac{\mathrm{d}^ny}{\mathrm{d}x^{n}}+a_{n-1}(x)\frac{\mathrm{d}^{n-1}y}{\mathrm{d}x^{n-1}}+\dots=y
$$


### Algebraic Solution
A differential equation can be solved using only algebra, and the standard value for $y$ will always be $e^{mx}$, as long as the differential equation has constant coefficients.
$$
\begin{align}
	y&=c_1e^{mx}\\
	y'&=c_2me^{mx}
\end{align}
$$

### Steps for solving
1. Verify that the differential equation has constant coefficients.
2. Find the characteristic equation.
3. Solve for $m$
4. Find the general form of the solution.

##### Example
Find a solution for the differential equation $2y'+5y=0$.

We replace $y$ with the general solution $e^{mx}$.
$$
2[me^{mx}]+5[e^{mx}]=0
$$

### Higher Order Differential Equation{s
The equation can be rewritten as
$$
ay''+by'+cy=am^2e^{mx}+bme^{mx}+ce^{mx}=0
$$
and we can solve for $m$ using the general formula for quadratics
$$
\begin{align}
  m_1=\frac{-b+\sqrt{b^2-4ac}}{2a} &&
  m_2=\frac{-b-\sqrt{b^2-4ac}}{2a}
\end{align}
$$

#### Example
Solve the differential equation $2y''-5y-3=0$.

We rewrite this using its general solution. Note that it's not necessary to write $e^{mx}$, since this term can never be equal to $0$.
$$
2m^2-5m-3=0
$$
Using the general formula, we solve for m
$$
\begin{align}
m_1=3 &&
m_2=-\frac{1}{2}
\end{align}
$$
Now that we have $m$, we have the general solutions of the equation
$$
y=c_1e^{3x}+c_2e^{-1/2}
$$
Note that this is only a general equation, since we haven't found the coefficients $c_1$ and $c_2$.

#### Example
Solve the differential equation $y''-10y'+25y=0$

The characteristic equation becomes
$$
m^2-10m+25=0
$$
We can see that this is a notable product of the form
$$
(m-5)^2=0
$$
Where the values of $m$ are
$$
m_1,m_2=-5
$$
Giving us the general solution
$$
y=c_1e^{5x}+c_2e^{5x}
$$
$e^{5x}$ should not be factorized out, since each of these terms represents a different physical phenomena.