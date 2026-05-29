---
tags:
  - Statistics
---

# Definition
A vector where elements are random variables

This could be from a random sample 

# Notes
$$
\begin{aligned}
E(\vec{Y}) &= \vec{\mu}\\
var(\vec{Y}) &= E[(\vec{Y}-\vec{\mu})(\vec{Y}-\vec{\mu})^T]
\end{aligned}
$$
the variance-covariance matrix has variance on the diagonal and covariance else where

## Linear combinations
Constant vectors can be factored out similar to univariate.
$$
\begin{aligned}
E(\vec{a}'\vec{Y}) &= \vec{a}'\vec{\mu}\\
var(\vec{a}'\vec{Y}) &= \vec{a}'E[(\vec{Y}-\vec{\mu})(\vec{Y}-\vec{\mu})']\vec{a}
\end{aligned}
$$
Reminder that we return to univariate when working with a linear combination

