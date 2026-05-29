---
tags:
  - Statistics
---


# Definition
Using the L1 and L2 norm are common methods of [[regularization]] to account for the [[Bias-Variance Tradeoff]]

# [[Linear Regression]]

Linear regression can be expressed as $\hat{\beta}^T X = \beta_0 + \beta_1x_1 + \dots + \beta_p x_p$ 

$$
\begin{aligned}
r &= y - \hat{\beta^T} X \\
\implies P(r = a) &= \text{Probability of measuring residuals as }a\\
&= \frac{1}{\sqrt{2\pi\sigma^2}}e^{-\frac{1}{2}(\frac{a}{\sigma})^2}\\\\
\hat{\beta} &:= \text{the weights that maximize the chances of observing the data}\\
\implies \hat{\beta} &= argmax_\theta P(X|\hat{\theta})\\
&= argmax_\theta \prod^n_{i=1} P(x_i,y_i|\theta), \text{independent observations}\\
\end{aligned}
$$

We can then optimize this to get the cost function
$$
\begin{aligned}
\hat{\beta} &= argmax_\theta \prod^n_{i=1} P(x_i,y_i|\theta)\\
&= argmax_\theta \prod^n_{i=1} log(P(x_i,y_i|\theta)), \text{monotonicity of logorithms preservse optimization goals}\\
&= argmax_\theta \prod^n_{i=1} [log(\frac{1}{\sqrt{2\pi\sigma^2}}e^{-\frac{1}{2}(\frac{y_i-\theta^T X}{\sigma})^2}],\\
&= argmax_\theta \prod^n_{i=1} [log(\frac{1}{\sqrt{2\pi\sigma^2}}) + -\frac{1}{2}(\frac{y_i-\theta^T X}{\sigma})^2]\\
&= argmax_\theta \prod^n_{i=1} [-(y_i-\theta^T X)^2], \text{removing constants}\\
\end{aligned}
$$
From this we get the Least Squares objective

## L2 Norm
Change the objective to maximize the probability of observing the data AND the parameters

## L1 Norm
Change the objective to maximize the probability of observing the data AND the parameters

# Related
- [What Textbooks Don't Tell You About Curve Fitting](https://www.youtube.com/watch?v=q7seckj1hwM)

