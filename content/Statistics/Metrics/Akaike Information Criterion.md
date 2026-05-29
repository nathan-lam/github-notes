---
tags:
  - Statistics/Theory
---

A heuristic used to tell if a model is over fit
Smaller = better

# Definition

$$AIC = -2log(likelihood)+2k$$
The loglikelihood will be small with a good fit, but it is "punished" by a big model, k = number of variables used


# Variations

## Bias Corrected AIC
Better for small sample sizes

$$AIC_{c}=AIC + \frac{2k(k+1)}{n-k-1}$$


# Resources


# Related
[[Bayesian Information Criterion]]
