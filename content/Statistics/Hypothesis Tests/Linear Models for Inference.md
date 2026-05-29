---
tags:
  - Statistics/Models/Linear
  - Statistics/Inference/Hypothesis-Tests
---

# Definition
[[Linear Models]] are a common tool to test whether there is strong relationship between a response and predictor.

Linear models allow for easy interpretation as we can read off coefficients as indicators of how significant the variables are.

Models are typically [[Linear Regression]] or [[Logistic Regression]]

# Assumptions
Assumptions for linear regression when used for [[Statistical Inference]].

## [[Linearity]]
There is a linear relationship between the response and predictors.

If this is false, then a transformation may be needed.

Plot a response vs predictor [[scatter plot]] to determine linearity.
## Independence
The residuals are independent.

If observations are independently measured, then the residuals tend to also be independent.

[[Time Series]] may have this issue due to [[Autocorrelation]]
- residuals are not independent if they are correlated in time

Plot a residuals vs time [[scatter plot]] to determine this.
## [[Homoscedasticity]]
Residuals have constant variance


A Fitted values vs residual [[scatter plot]] can determine this as there should be no cone shape in the plot
- The cone is the variance changing as the fitted values change.

## Normality
Residuals should be roughly normally distributed.
- The central limit theorem kicks in when n > 30

A QQ norm plot can be used to verify this.

# Hypothesis Tests
A linear model has multiple quantities that are good candidates for hypothesis testing.

## Coefficients
$\hat{\beta} \sim Normal((X^TX)^{-1}X^TY, (X^TX)^{-1}\sigma^2)$


## F Test


# Reading a model summary

Statistical software will often include a table of summary statistics.

## Regression

| Variable    | estimate | std.error | statistic | p.value |
| ----------- | -------- | --------- | --------- | ------- |
| (Intercept) |          |           |           |         |
| x_0         |          |           |           |         |
This table shows the predictors in a linear model
- Estimate = coefficient of that variable in the model
- std.error = standard deviation of the estimate
- statistic = t statistic
- p.value = p value of the estimate

## Classifier



# Related
- https://www.statology.org/linear-regression-assumptions/
- [[Linear Regression Coefficient Solution]]