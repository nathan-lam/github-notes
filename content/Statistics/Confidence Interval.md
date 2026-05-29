---
tags:
  - Statistics/Inference
---

# Definition
An interval that has a defined % chance of capturing the true value.

It takes the form of 
center value - k* standard error< true value < center value + k* standard error
- k is the dial we chance the coverage of confidence

# Derivation

$$
\begin{aligned}
P(-c<T<c) &= \alpha &, \text{Find boundaries }(a,b)\text{such that the probability is }\alpha\\
&= P(\bar{x}-\frac{cS}{\sqrt{n}}<\mu<\bar{x}+\frac{cS}{\sqrt{n}}), &T=\frac{\bar{x}-\mu}{S/\sqrt{n}}\\

\end{aligned}
$$

# Related
- [[Hypothesis Tests]]
	- This is equivalent to a hypothesis test
- [[Prediction Interval]]
- [[Bootstrapping]]
	- It is common technique to estimate a confidence interval using bootstrapping
