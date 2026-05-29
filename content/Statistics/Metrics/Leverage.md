---
tags:
---

# Definition
A measure of how unusual a data point is to the group in [[Linear Regression]] as a method of outlier detection.


# Hat Matrix
We measure a point's influence based on the hat matrix

$$
\begin{aligned}
\hat{Y} &= X\hat{\beta}\\
&= X(X^TX)^{-1}X^TY\\
\hat{Y} &= HY, H = X(X^TX)^{-1}X^T\\
h_{ii} &= \text{Mahalanobis Distance; standardized distance to the mean}
\end{aligned}
$$

# Influence

Influence is the specific metric of how much the coefficient changes when a point is removed.

Influence = Outlyingness * leverage
$$
D_i = || \hat{\beta}_{\text{w/ ith point}} - \hat{\beta}_{\text{w/o ith point}}||^2
$$

