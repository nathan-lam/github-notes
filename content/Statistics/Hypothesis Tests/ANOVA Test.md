---
hypothesis_distribution: F
hypothesis_parameter:
tags:
  - Statistics/Hypothesis-Test
---
ANalysis Of VAriance (ANOVA)

# Application
To compare 3 or more groups/categories on a numerical variable


# Hypothesis
$$H_{0}: \mu = c$$
$$H_{A} : \mu \neq c$$

Each group differs by an off set but have the same spread
or 
Each group has the same mean or there is at least 1 difference

# Variations
ANOVA is similar to linear regression in that it takes 1 or 2 categorical variables and outputs a numerical variable. Keep in mind this is not for prediction

## One Way ANOVA

Tests 1 independent variable

Ex. Test scores between age groups
- Independent var: Age Group (categorical)
- Dependent var: Test scores (numerical)

## Two Way ANOVA
Tests 2 independent variable

Ex. Test scores between age groups
- Independent var: College Major (categorical), Ethnicity (categorical)
- Dependent var: Median Income (numerical)

keep in mind that the hypothesis here is a statement about difference in (college major, ethnicity) pairs


# Applications

## Alternative to Linear Regression
ANOVA is basically a linear regression with continuous output, categorical input

## Linear Regression Coefficients
Alternative to performing multiple t-tests for each regression coef
Null: The
Alt: There is at least 1 variable not 

## Comparison between Models
Comparing the sum of squares error between models on the same dataset
Null: They are the same
Alt: They are NOT the same


# Derivation

ANOVA follows an F test, meaning it's the ratio of 2 Chi Squared tests

We are checking if the variance within a group is the same as the variance between the groups


# Assumptions
- Normality
- Constant Variance
- Independent between groups
- Independence between observations



# Related
- [[MANOVA Test]] - if multiple dependent variables are desired
- [Analysis of Variance | Statistics Ep. 26](https://www.youtube.com/watch?v=qP7rqPeQGBI)
