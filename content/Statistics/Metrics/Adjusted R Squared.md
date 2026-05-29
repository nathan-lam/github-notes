---
tags:
  - Statistics/Theory
---

# Definition
An adjustment to the [[R Squared]] metric as it becomes less helpful when using multiple predictors.

$$
\begin{aligned}
R^{2}&= 1 - \frac{\text{Error sum of squares}}{\text{Total sum of Squares}}\cdot\frac{n-1}{n-k-1}\\
&= 1-\frac{\sum(y-\hat{y})^2}{\sum\limits(\bar{y}-\hat{y})^2}\cdot\frac{n-1}{n-k-1}\\
&= 1 - \frac{var(errors)}{var(y)}\cdot\frac{n-1}{n-k-1}\\
\end{aligned}
$$

The goal is to reduce the R squared from inflating as the number of predictors (k) increases
