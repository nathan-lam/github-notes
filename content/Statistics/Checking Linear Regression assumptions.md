---
tags:
  - Statistics/Models/Linear
---

# Definition

[[Linear Regression]] has several assumptions
![[Linear Models for Inference#Assumptions]]


# Checks and Fixes

| Issue                | Primary check                     | Primary Fix                                        |
| -------------------- | --------------------------------- | -------------------------------------------------- |
| nonlinearity         | residual plot; vs. regressor plot | transformations; nonlinear models                  |
| nonconstant variance | residuals vs fitted plot          | transformations; bootstrap cases; robust std error |
| not independent      | not considered                    | depends                                            |
| non normality        | QQ plot                           | transformations; any bootstrap                     |


