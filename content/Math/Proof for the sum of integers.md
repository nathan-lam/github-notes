---
tags:
  - Mathematics/Proofs
---

# Definition
The sum of the first n integers can be expressed as a polynomial.
$$\sum^n_{k=1} k = S_n = \frac{n(n+1)}{2}$$

# Proof

[[Proof By Induction]]

## Base case
$$
\begin{aligned}
k=1 \implies S_1= 1\\
\frac{(1)(1+1)}{2} = 1 \implies \text{Base case works}
\end{aligned}
$$

## n+1 case

$$
\begin{aligned}
S_{n+1} &= (n+1) + S_n\\
&= (n+1) + \frac{n(n+1)}{2}\\
&= (n+1)(1 + \frac{n}{2})\\
&= (n+1)(\frac{2+n}{2})\\
&= \frac{(n+1)(n+2)}{2}
\end{aligned}
$$

