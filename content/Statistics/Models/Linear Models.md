---
tags:
  - Statistics/Models/Linear
---

# Definition
A class of statistical models that rely on a linear relationship between the response and predictors.


# Workflow



# Tools
Creating a good linear model tends to require the data to be massaged into place. 

## Nonlinear Transformations
A common issue is that real data is not always linear, but sometimes there are ways to transform them so they become linear.

Note that transformations makes inference harder to understand as it is not easily interpretable.

A log transform has some limited interpretation as a log is roughly the % change.
- This is because $log(x) \approx x$ for small x
### Log Response Model
A log transform only on the response.

In regression, this represents an exponential relationship.
- Roughly represents a ($\beta\times 100$)% change in Y given 1 unit change in X

### Log Predictor Model
A log transform only on the predictors.

In regression, this represents a logarithm relationship.
- Roughly represents a ($\frac{\beta}{100}$) unit change in Y given 1% change in X

### Log-Log Model

A log transform on both the response and predictors.

Roughly represents a $\beta$% change in Y given 1% change in X

## One Hot Encoding
Categorical variables are [[One Hot Encoding|One Hot Encoded]] 

## Interaction terms
Some predictors may include additional effects when interacting. This is representing as a new predictor the multiplies both predictors together, $X_i\cdot X_j$

### Numerical x Numerical


### Numerical x Categorical
Represents a change in trajectory depending on the state of the categorical variable.

### Categorical x Categorical


## Variable Selection
A set of techniques that helps pick out significant predictors from a set of predictors.

Generally aim for smaller models.


# Related
- 
- Kernel Trick

