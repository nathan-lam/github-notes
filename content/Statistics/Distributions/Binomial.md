---
statistics_parameters: $(n, p)$
statistics_pdf:
statistics_cdf:
statistics_mean: $np$
statistics_variance: $np(1-p)$
tags:
  - Statistics/Models/Distributions
---

# Definition





# Related
- Sum of [[Independent and Identically Distributed|iid]] [[Bernoulli]] samples
$$
\begin{aligned}
\text{Let }A &\sim Bernoulli(p)\\
X &= \sum^n_{k=1} {n\choose k} p^n (1-p)^{n-k}\\
\implies X &\sim Binomial(n,p)
\end{aligned}
$$
