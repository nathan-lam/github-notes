---
tags:
---

# Definition
Residuals are the observed errors of a [[Linear Regression]] model.
$$Residuals = true model - fitted model = f(x|\theta) - \hat{f}(x|\hat{\theta})$$

The model explains some amount of of the data and the errors are the accumulation of all unexplained behavior, which makes the [[Central Limit Theorem]] reason that the [[Normal]] distribution as a reasonable approximation.

We assume the residuals have the same properties as the errors
$$
\begin{aligned}
e_1,e_2, ... , e_n iid \sim Normal(0,\sigma^2)
\end{aligned}
$$



## Estimates

We expect the mean to sum to zero on average, and the [[Mean Squared Error]] to estimate the variance.

$$
\begin{aligned}
e_i &= y_i = \hat{y}_i\\
sd(e) &= \frac{1}{n}\sum (e_i - \bar{e})^2\\
&= \frac{1}{n}\sum e_i^2\\
&= MSE
\end{aligned}
$$






# Related
- [[residuals vs fitted plot]]
- [[Standardized Residuals]]
- [[The Data Vector is Orthogonal to the Residuals]]


