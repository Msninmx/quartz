---
title: Subsets
disableToc: true
---

### Subsets
When dealing with [[notes/set-theory|sets]], we can say that certain sets are _subsets_ of other sets.

$A$ is a subset of $B$ if and only if every element in $A$ is also an element of $B$.
$$A \subseteq B$$
If not:
$$A \nsubseteq B$$
In this example $B$ is the superset of $A$.
$$B \supseteq A$$
If $B$ has more elements than $A$, $A$ is a proper subset of $B$.
$$A \subset B$$

The [[notes/null-set|null set]] is a subset of every other set.
$$\emptyset \subseteq A$$

Every set $A$ is a subset of itself.
$$A \subseteq A$$
Equal sets are marked with an equals sign.
$$A = B$$
A power set of a set is every set that can be made from its elements.
$$
\begin{align}
	A &= \{a, b\} \\
	P(A) = \{ &\emptyset, \{a\}, \{b\}, \{a, b\} \}
\end{align}
$$
#logic #setTheory 
