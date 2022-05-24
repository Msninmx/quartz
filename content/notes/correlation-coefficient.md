---
title: "Correlation Coefficient"
disableToc: true
---
### Correlation Coefficient
Correlation is a measurement that determines if a variable can be a function of another. This is useful in determining whether or not a given variable actually effects the end result.

The formula for the correlation coefficient is:
$$
r=\frac{\sum_{i=1}^{N}(x_i-\overline{x})(y_i-\overline{y})}
{\sqrt{\sum^{N}_{i=1}(x_i-\overline{x})^2}
\sqrt{\sum^{N}_{i=1}(y_i-\overline{y})^2}}
$$
Where:
- $x_i$ is $x$ value of each independent variable.
- $y_1$ is the $y$ value of each dependent variable.
- $N$ is the number of data points.
- $\overline{x}$ is the average of the $x$ values.
- $\overline{y}$ is the average of the $y$ values.

$r$ can have a value between $-1$ and $1$, where the sign of $r$ determines if there's a positive or negative correlation.

If $-0.5 \leq r\leq 0.5$, then there exists a weak correlation. If $-0.8 <r< -0.5$ or $0.5 <r< 0.8$ then there exists a moderate correlation. If $-0.8>r$ or $0.8<r$, then there exists a strong correlation.