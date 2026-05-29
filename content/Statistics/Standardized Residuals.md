---
tags:
  - Statistics/Models/Linear
  - Statistics/Theory
---

# Definition
A transformation on observed residuals to become standardized.
$$e_i\sim Normal(0,\sigma^2) \implies \frac{e_i}{\sigma}\sim Normal(0,1)$$
It effectively turns the quantity into a z score.


## Studentized Residuals

Because the true variance is not known, we can use the sample variance to "studentize"

$$t_i = \frac{\hat{e}}{\hat{\sigma}\sqrt{1-h_{ii}}}$$



# [[Outlier Detection]]
Standardized residuals is one way to detect outliers.


A data point is a statistical [[Outliers|outlier]] if it has high [[leverage]] and high z score.
- Rule of thumb: High z score $\implies$ z > 3


# Related
- [Standardized and Studentized Residuals](https://www.bohrium.com/en/sciencepedia/feynman/statistical_learning_undergraduate-standardized_and_studentized_residuals)
