---
title: "Differential Equations"
disableToc: true
---
### Differential Equations
A differential equation is any equations that contains the derivative of one or more unknown functions.
$$
   a_n(x)\frac{\mathrm{d}^ny}{\mathrm{d}x^{n}}+a_{n-1}(x)\frac{\mathrm{d}^{n-1}y}{\mathrm{d}x^{n-1}}+\dots=y=g(x)
$$


Normally we work with functions, either graphing them or solving them. However, sometimes we don't have access to this function, only the derivative of the function. Solving a differential equation consists of finding this original equation.

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


### Second Order Differential Equation{s
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
Depending on the value of the discriminant $(b^2-4ac)$, the solution will take on different forms:
$$
\begin{align}
1.\quad b^2-4ac>0,&\qquad y=c_1e^{m_1x}+c_2e^{m_2x} \\
2.\quad b^2-4ac=0,&\qquad y=c_1e^{mx}+c_2xe^{mx} \\
3.\quad b^2-4ac<0,&\qquad y=e^{\alpha x}\left[c_1\cos\beta x+c_2\sin\beta x\right],\quad\text{where}\quad m=\alpha\pm\beta i
\end{align}
$$

##### Example
Solve the differential equation $2y''-5y'-3y=0$.

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

##### Example
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

#### Types of Solution
The solution of a DE is composed by:
- A complementary solution, $y_c$
	- Its always multiplied by $c$, and is usually transient.
- A particular solution, $y_p$
	- Is not multiplied by $c$, and is found by solving the non-homogeneous equation (when the equation is equal to $0$).

In other words, the complementary solution is a vague solution to the DE, in these examples all the solutions we have found have had complementary solutions since the right hand side of the equations has been equal to $0$. When this part is not equal to $0$, we are looking for a particular solution, where the coefficients are defined.

##### Example
Find the solution, $y$, for the DE:
$$
y''+4y'+7y=2
$$
First, we'll solve the homogeneous equation, e.i, the left hand part equalized  to $0$.
$$
y''+4y'+7y=0
$$
Solving this using the characteristic equation we get:
$$
m^2+4m+7=0, \quad m=-2\pm\sqrt{3}i
$$
Since our value for $m$ is a complex number, we have a specific form for our solution.
$$
\begin{align}
\alpha = -2 &\qquad \beta=\sqrt{3}\\\\
y_c=&e^{-2x}\left[c_1\cos\sqrt{3}x+c_2\sin\sqrt{3}x\right]
\end{align}
$$
This is our complementary solution. The method we will use to find the particular solution is called the Undetermined Coefficients Method. We will assume that $y_p$ looks similar to what we have to the right of the equal sign. In this example, $y_p$ should be a constant, since what's on the right hand side of the equation $2$, is also constant. With this assumed value of $y_p$ we can find assumed values for $y_p'$ and $y_p''$
$$
y_p=A\quad y_p'=0\quad y_p''=0
$$
With these values for $y$, we can substitute these into our original DE to find the value of $A$, which will be $2/7$, which also becomes the value of our particular solution.

We can now find the general solution to the DE, defined as $y=y_c+y_p$
$$
y=e^{-2x}\left[c_1\cos\sqrt{3}x+c_2\sin\sqrt{3}x\right]+\frac{2}{7}
$$