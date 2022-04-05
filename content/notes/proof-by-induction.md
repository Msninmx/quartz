---
title: Proof by Induction
disableToc: true
---

### Proof by Induction
##### Example
Prove using induction:
$$
P(n)=1+2+3+\dots + n = \frac{n(n+1)}{2}
$$

First, we prove its true for a base case
$$
P(1)=\frac{1(2)}{2}=1
$$
Then we assume that $n=k$, $n$ is equal to some number $k$
$$
P(k)=1+2+3+\dots+k=\frac{k(k+1)}{2}
$$
Then we check if this is still true for its successor $k+1$
$$
P(k+1)=1+2+3\dots+k+(k+1)=\frac{(k+1)((k+1)+1)}{2}
$$
We see that what's on in the middle part of the equation can be simplified as our case for $k$
$$
\frac{k(k+1)}{2}+(k+1)=\frac{(k+1)(k+2)}{2}
$$
We continue to simplify terms to check if both sides are equal
$$
\begin{align}
	(k+1)(\frac{k}{2}+1)&=\frac{(k+1)(k+2)}{2} \\
	(k+1)(\frac{k+2}{2})&=\frac{(k+1)(k+2)}{2} \\
	\frac{(k+1)(k+2)}{2}&=\frac{(k+1)(k+2)}{2} \\
\end{align}
$$
Since this outcome is true, our initial statement is true.

#logic 
