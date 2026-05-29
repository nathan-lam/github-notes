---
tags:
  - Statistics/Theory
  - Algorithms/Bootstrapping
---
A computational method of estimating parameters from a sample
- Sample from the sample with replacement

# Assumptions
It is assumed the sample is a good representation of the population



# Application

## Estimating variance
1. Prepare 1000 bootstrapped results
2. For each bootstrap
	1. Calculate the variance
3. Now we have 1000 bootstrapped variances
	1. This can be treated as the distribution of the sample variance
4. Taking the mean and variance of the bootstraps gives the estimated mean and variance
5. The 225th and 975th percentiles give the 95% confidence interval


