---
title: Natural Deduction
disableToc: true
---

### Natural Deduction
[[notes/logic|Logic]] allows us to infer, through simple syntactical manipulation, new ideas from old ones.

An argument is formed through a series of initial statements call Premises. It is considered valid if its premises are valid.

##### Example
Verify if the following syllogisms are valid using a truth table:
$$
\begin{align}
	p \to&(q \lor \neg r) \\
	q \to&(p \land r) \\
	\therefore p \to& r
\end{align}
$$
We evaluate the value of our two premises and compare it to the value of the conclusion. When the two premises are true, the conclusion must be true as well. In this example, it's false.

#logic 
