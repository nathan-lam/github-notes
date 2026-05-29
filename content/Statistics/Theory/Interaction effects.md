---
tags:
  - Statistics/Inference
---
Interactions are when 2 inputs play a bigger role together than individually

This works for any combination of numerical and categorical variables together

# How to do it?
This looks like multiplying the two variables together


# Types of Interactions
The TL;DR is that the total is greater than the sum of its parts
A, B affecting C has an extra kick working together than individually

## Numerical x Numerical
The coefficient says that the trajectory changes in a gradient as one variable changes
There is a continuum of possible slopes

## Categorical x Numerical
The coefficient says how the trajectory on the numerical variable changes when the 
Ex. 
- If On, goes upward
- if Off, goes downward

## Categorical x Categorical
The coefficient means that when both are on, there's a bigger effect

Ex. $aA + bB + cA*B = (a+c)A + (b+c)B$ if both are on
One categorical kicks up the intercept, the interaction of 2 categories kicks up the intercept more than individually

# Interpretation
1. Verify that it is significant, good p-value (there is a statistical difference)
2. Verify if it is different without it, passes ANOVA comparison (there is a difference)


# Caution
Don't add interaction effects everywhere as more may overfit the model
This is why the ANOVA test is used to really see if there's a difference
- dont use it if we dont have to

# Related

