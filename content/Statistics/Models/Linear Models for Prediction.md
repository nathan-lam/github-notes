---
knowledge_classes:
  - UCLA-stat401
  - UCLA-stat402
  - UCB-stat151a
tags:
  - Statistics/Models/Linear
---

# Definition
[[Linear Models]] are great tools for prediction. The goal is increase the correctness of the model

This is typically done by addressing the [[Bias-Variance Tradeoff]].
- Linear models for inference have low bias but high variance
- We increase predictive ability by increasing bias to decrease variance

# Ways to decrease variance


## Regularization
Bias is added to help simplify the model and signify which features are most important

### Ridge
A penalizer that uses the L2 norm of the slopes

The modified cost function becomes:
$C = \sum (y-\hat{y})^{2}+\lambda||\beta||_2$
The penalized slopes will approach zero but never reach zero

### LASSO
A penalizer that uses the L1 norm of the slopes

The modified cost function becomes:
$C = \sum (y-\hat{y})^{2}+\lambda||\beta||_1$
Using the L1 norm allows the slopes to reach zero

### Elastic Net
A combination of both LASSO and Ridge

## [[Cross Validation]]
Test the model performance using cross validated test sets

# Theory
$\vec{Y} = X\beta+\vec{\epsilon}$ where $X\beta$ is fixed and $\epsilon$ is random

The Gauss-Markov conditions means 
- $\epsilon \sim Normal(0,\sigma^{2}I)$ 
	- Mean zero
	- same constant variance
	- independent/uncorrelated errors

$\vec{\epsilon} \sim Normal(0,\sigma^{2}I)\implies \vec{Y}\sim Normal(X\beta,\sigma^{2}I)$
- Because Y is just epsilon shifted

$\vec{\hat{\beta}} = (X^{T}X)^{-1}X^{T}\vec{Y}$
$\vec{\hat{\beta}}\sim Normal(\beta,(X^{T}X)^{-1}X^{T}(X\beta + \epsilon))=Normal(\beta,\sigma^2(X^{T}X)^{-1})$

$\vec{\hat{Y}} = X\vec{\hat{\beta}} = X(X^{T}X)^{-1}X^{T}\vec{Y}= H\vec{Y}$
$\vec{\hat{Y}}\sim Normal(HX\beta,\sigma^{2}I) = Normal(X\beta, \sigma^{2}I)$


# Related
[[Supervised Learning Models]]