---
title: "Variance"
disableToc: true
---
### Variance
Variance is an indicator that shows us how far away we are from a [[notes/expected-value|expected value]], and is defined as:
$$
\hat{\sigma}^2 \frac{\Sigma_{i=1}^{N}(x_{i}-\overline{x})^2}{N-1}
$$
##### Example
Given the grades of a student being:
$$
100, 100, 90, 100
$$
find the variance of their grades.

Substituting values into our formula:
$$
  \hat{\sigma }^2=\frac{(x_{1}-\overline{x})^2+(x_2-\overline{x})^2+\dots+(x_4+\overline{x})^2}{4-1}
$$
Where each value of $x$ is one of the grades and $\overline{x}$ is the average.
$$
\hat{\sigma}^2=25
$$