---
statistics_parameters: $df$
statistics_pdf:
statistics_cdf:
statistics_mean: n
statistics_variance: 2n
tags:
  - Statistics/Models/Distributions
---

# Definition





# Related
- Chi Squared is the sum of n standard [[Normal]] distributions
$$
\begin{aligned}
\text{A} \sim N(0,1)\\
\chi^2_n = \sum^n_{i=1} A^2_i\\
\end{aligned}
$$
- Sum of errors squared follows a Chi Squared Distribution
$$
\begin{aligned}
\text{Given } \epsilon_i \sim Normal(0,\sigma^2)\\
\implies \frac{\epsilon_i}{\sigma} \sim Normal(0,1^2)\\
\implies \sum^n_{i=1} (\frac{\epsilon_i}{\sigma})^2 \sim \chi^2_{n}\\
\therefore \frac{1}{\sigma^2} \sum^n_{i=1} \epsilon_i^2 \sim \chi^2_n
\end{aligned}
$$
- Sum of residuals squared follows a Chi Squared Distribution
- $$
\begin{aligned}
\text{Given } e_i \sim Normal(0,\sigma^2)\\
\implies \frac{e_i}{\sigma} \sim Normal(0,1^2)\\
\implies \sum^n_{i=1} (\frac{e_i}{\sigma})^2 \sim \chi^2_{n}\\
\therefore \frac{1}{\sigma^2} \sum^n_{i=1} e_i^2 \sim \chi^2_n
\end{aligned}
$$
TODO explain why sample residuals follows n-1 degrees of freedom, but population residual follows n degrees of freedom