---
tags:
  - Statistics/Derivations
  - Statistics/Models/Linear
---
# Statement
$$
\begin{aligned}
\hat{\beta} &= (X^TX)^{-1}X^TY\\
\hat{\beta} &\sim Normal((X^TX)^{-1}X^TY, (X^TX)^{-1}\sigma^2)
\end{aligned}
$$

# Given
$$
\begin{aligned}
Y &= X\beta + \epsilon\\
Y &= \text{Response Vector}\\
X &= \text{Data Matrix}\\
\beta &= \text{Coefficient vector}\\
\epsilon &= \text{White Noise Vector}\\
\end{aligned}
$$

# Derivation

## $\beta$ Solution
The solution involves different approaches to minimizing the loss function: $Loss = \sum^n_{i=1} ( y_i - \hat{y}_i)^2$

### Method of Least Squares


### Vector Calculus
$$
\begin{aligned}
Loss &= \sum^n_{i=1} ( y_i - \hat{y}_i)^2\\
&= (Y-\hat{Y})^T(Y-\hat{Y}), &\text{Convert summation to a vector product}\\
&= Y^TY-Y^T\hat{Y}-\hat{Y}^TY + \hat{Y}^T\hat{Y}, &\text{Distribute}\\
&= Y^TY-Y^TX\beta-(X\beta)^TY + (X\beta)^TX\beta, &Y=X\beta\\
\frac{\partial Loss}{\partial \beta} &= 0 - Y^TX - X^TY + 2X^TX\beta, &\text{take derivative in }\beta\\
&= 0 - 2X^TY + 2X^TX\beta, &Y^TX=X^TY \text{ because they are scalar values that multiply the same quantity}\\
0  &= 0 - 2X^TY + 2X^TX\beta, &\text{ set }\frac{\partial Loss}{\partial \beta}=0\\
2X^TY &= 2X^TX\beta\\
(X^TX)^{-1}X^TY &= \beta\\
&\therefore \beta = (X^TX)^{-1}X^TY
\end{aligned}
$$

## $\beta$ Distribution
$$
\begin{aligned}
\epsilon = \text{white noise} &\implies \epsilon\sim Normal(0,\sigma^2)\\
&\implies Y \sim Normal( X\beta, \sigma^2), \text{Linearity preserves normality}\\
&\implies (X^TX)^{-1}X^TY \sim Normal( (X^TX)^{-1}X^T(X\beta), (X^TX)^{-1}X^T\sigma^2X(X^TX)^{-1}), \text{multiply } (X^TX)^{-1}X^T \text{ to }Y\\
&\implies (X^TX)^{-1}X^TY \sim Normal(\beta, (X^TX)^{-1}\sigma^2)\\
&\implies \hat{\beta} \sim Normal(\beta, (X^TX)^{-1}\sigma^2)\\
\end{aligned}
$$

