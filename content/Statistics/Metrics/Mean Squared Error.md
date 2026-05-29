---
tags:
  - Statistics/Theory
---

# Definition
A cost metric used to measure how well an estimate is to the true value.
$$
\mathbb{E}[(\theta-\hat{\theta})^2]
$$
A measure of how different an estimate ($\hat{\theta}$) is from the true value ($\theta$)
It is squared as it is smooth and gets rid of negatives



# Bias-Variance
MSE can be decomposed as
$$
MSE = var(\hat{\theta}) + bias(\hat{\theta})^2
$$
Which highlights the bias-variance trade off


# Related
- [[Bias-Variance Tradeoff]]
- [[Root Mean Squared Error]]
	- Squaring punishes wrong answers more the further they are from the true value 
	- Square rooting reduces this punishment of errors
- [[Variance]]
	- The mean minimizes the squared distance for all samples. 
	- $E[(\theta - \bar{\theta})^2] = Var(\theta)$
- [[Mean Absolute Error]]
- https://en.wikipedia.org/wiki/Bias%E2%80%93variance_tradeoff

