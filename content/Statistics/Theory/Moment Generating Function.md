---
tags:
---

# Definition
$$

M_{X(t)}= E(e^{tX})
$$
We encode the centered [[Moments]] as the coefficients of the exponential [[04 Notes/Field of Study/Math/Taylor Series]] which can be compressed into a [[Generating Functions|generating function]]

# Notes

$$
\begin{aligned}
\text{Let }ln(M_{X(t)})= \phi(t)\\
\implies \frac{\partial}{\partial t_{i}}\phi(t=0)=\phi_i(0) = E(X)\\
\implies \frac{\partial}{\partial t_{i}^{2}}\phi(t=0) =\phi_{ii}(0) = var(X)\\
\implies \frac{\partial}{\partial t_{i}\partial t_{j}}\phi(t=0)=\phi_{ij}(0) = cov(X_i,X_j)\\
\end{aligned}
$$

If we are working with a random vector, then it's the same but with vectors
$M_{\vec{X}}(\vec{t}) = E(e^{\vec{t}^{T}\vec{X}})=E(e^{\sum^{n}_{i=1} t_iX_i})$
We are still summing them up despite this not being a transformation that sums all the elements

If we start with with a MGF of a random vector, we can select a specific element by setting all other t to 0

## Theorems
If X and Y have the same MGF, then they have the same distribution




