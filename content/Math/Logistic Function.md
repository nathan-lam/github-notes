---
tags:
  - Mathematics/Functions
aliases:
  - Sigmoid Function
---

# Definition
A function that describes an initial exponential growth and plateaus to a maximum carrying capacity.

$$
\begin{aligned}
f(x) &= \frac{L}{1+e^{-k(x-x_0)}}\\
L &= \text{Maximum Carrying Capacity}\\
k &= \text{Growth Rate}\\
x_0 &= \text{Midpoint}\\
\end{aligned}
$$

This maps $(-\infty,\infty) \to [0,1]$ 

# Notes

## [[Logistic Regression]]
This maps a linear combinations to a probability


## [[Neural Networks]]
This was one of the first tried nonlinear activation functions as it had an easy closed form derivative for [[Backpropagation]]


# Related

