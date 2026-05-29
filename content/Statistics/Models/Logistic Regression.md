---
tags:
  - Statistics/Models/Linear
---

# Definition
A [[Linear Models|Linear Model]] that assumes the log-odds of the response (Y) is a [[Linear Combination]] of the predictors (X).

$$
\begin{aligned}
log(\frac{p}{1-p}) &= a_1X_1 + a_2X_2 + \dots + \epsilon\\
p &= \text{Probability of the Response variable}\\
a_i &= \text{Coefficients}\\
X_i &= \text{Predictor Variables}\\
\epsilon &= \text{Residuals or White Noise}
\end{aligned}$$
The probability corresponds to a binary outcome. If multiple outcomes are involved, then it becomes a [[Multinomial Logistic Regression]]. 


The model becomes $$P(Y|X) = \frac{1}{1+exp(-[a_1X_1 + a_2X_2 + \dots + a_pX_p])}$$


# Notes
Logistic Regression can be used as a [[Linear Models for Inference|hypothesis test for inference]] or for [[Linear Models for Prediction|prediction]]

This is the simplest [[Neural Networks|neural network]] as it has no hidden layers and a [[Logistic Function|logistic]] activation function

# Related
- [[Linear Regression]]
- [[Ordinal Regression]]
