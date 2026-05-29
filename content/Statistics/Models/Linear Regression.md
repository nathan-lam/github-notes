---
tags:
  - Statistics/Models/Linear
aliases:
  - Ordinary Least Squares
---

# Definition
A [[Linear Models|Linear Model]] that assumes the response (Y) is a [[Linear Combination]] of the predictors (X).

$$
\begin{aligned}
Y &= a_1X_1 + a_2X_2 + \dots + \epsilon\\
Y &= \text{Response variable}\\
a_i &= \text{Coefficients}\\
X_i &= \text{Predictor Variables}\\
\epsilon &= \text{Residuals or White Noise}
\end{aligned}
$$

The model becomes 
$$
\begin{aligned}
E(Y|X) = a_1X_1 + a_2X_2 + \dots + a_pX_p\\
\end{aligned}
$$

# Notes
Linear Regression can be used as a [[Linear Models for Inference|hypothesis test for inference]] or for [[Linear Models for Prediction|prediction]]
- If used for inference then the inference assumptions must be true.


If the data matrix (X) has no [[Multicollinearity]] then the coefficients have a unique closed formed solution.
$$\hat{\beta} = (X^TX)^{-1}X^TY$$

This is the simplest [[Neural Networks|neural network]] as it has no hidden layers and a linear activation function
# Related
- [[Logistic Regression]]

