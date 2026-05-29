---
tags:
---
A L1 norm penalizer
Adds bias to reduce variance

# Definition
In a linear model, a Lasso penalizer is
$$
\hat{\beta} = argmin_{\hat{\beta}} f(x|\hat{\beta}) + \lambda ||\hat{\beta}||_1
$$
Where lambda is a scaler for the intensity of the penalizer

# Assumption
- Statistical inference is no longer desired
	- Added bias means coefficients do not correspond to the true values, which the hypothesis tests are aiming for



# Related

