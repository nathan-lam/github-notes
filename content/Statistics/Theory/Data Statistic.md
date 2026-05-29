---
tags: Statistics
---

# Definition
A statistic is a calculation based on a sample.
Ex. mean, median, mode
but we want one with good properties


# Types of Statistics

## Unbiased Estimator (statistic)
On average, the estimator hits the true parameter value

## Sufficient Statistic
No other statistic can provide additional information from a given sample.

Sufficiency properties
- A function of a sufficient stat is also sufficient

Minimum Sufficiency

Notes
- MLE estimators are functions of sufficient stats

## Efficiency
Minimum variance unbiased estimator
An estimator has the lowest possible variance

Efficient if 
$$
\frac{1}{I_n(\theta)} = var(\hat{\theta})
$$
This is the Cramer Rao Lower bound using the fisher information. A ratio
$$
\begin{align}
I_n(\theta)&=nI_1(\theta)\\ 
I_1(\theta)&=E[(\frac{\partial}{\partial\theta}lnf(x))^{2}]= -E[\frac{\partial^2}{\partial\theta^2}lnf(x)]
\end{align}
$$

Efficiency Ratio is also used to compare

# Consistency
An estimator becomes more accurate as more data is used. (Weak law of large numbers)

$$
\lim_{n\to\infty}P(|\hat{\theta-\theta|>\epsilon})=0
$$