---
tags:
  - Statistics
---

# Definition
Random variables dependent on other random variables

$X|Y \sim A$
$Y \sim B$


$f_{X(x)}= \int^{\infty}_{-\infty}P(X=x,Y=y)dy = \int^{\infty}_{-\infty}P(X=x|Y=y)P(Y=y)dy$
- basically integrating out the Y
- 
$E(X) = E[E(X|Y)]$
$var(X) = E[var(X|Y)]+var(E[X|Y])$
