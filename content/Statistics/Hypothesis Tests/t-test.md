---
hypothesis_distribution: "[[t]]"
hypothesis_parameter: df
tags:
  - Statistics/Hypothesis-Test
aliases:
  - Student's t-test
---

# Definition
 A hypothesis test used to compare a test statistic that has been shifted and scaled.

A test statistic follows a t-distribution if the quantity is represented as:
$$
\begin{aligned}
\text{Given:}&\\
Z&\sim Normal(\mu,\sigma^2)\\
(n-1)\frac{s^2}{\sigma^2}&\sim \chi^2_{n-1}\\
\implies
\frac{(\frac{Z-\mu}{\sigma})}{\sqrt{\frac{(n-1)\frac{s^2}{\sigma^2}}{n-1}}} = \frac{Z-\mu}{s} &\sim t_{n-1}\\
\end{aligned}
$$
In simpler terms, the t distribution is a ratio of $\frac{\text{Standard Normal}}{\sqrt{\frac{\text{Chi Squared}}{n}}}$

The test statistic is similar to standardizing a random variable except we use a standard deviation estimate instead of the true standard deviation.


# Properties
- $\lim_{n\to\infty} t_n = Normal(0,1)$
	- This is in addition to the [[Central Limit Theorem]]


# Application
To evaluate if the a random variable is statistically equivalent to a guess

# Hypothesis
$$H_{0}: \mu = c$$
$$H_{A} : \mu \neq c$$
# General Assumptions
- Independent samples
- Data is normally distributed
	- If n > 30, then the [[Central Limit Theorem]] kicks in. This means normal-ish data can still work
		- Note that sample variance estimate may be affected by non-normal data, but will be less affected as n increases for different reasons
- Standard deviation is unknown
- Data is continuous

# Variations

| Version                     | Test Statistic                                                                                     | Degrees of Freedom                                                                                                                                                                 | Assumptions                                                              |
| --------------------------- | -------------------------------------------------------------------------------------------------- | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------------------------------------------------------------------ |
| 1 Sample t-test             | $\frac{\bar{x}-\mu}{\frac{s}{\sqrt{n}}}$                                                           | n-1                                                                                                                                                                                |                                                                          |
| Independent 2 Sample t-test | $\frac{(\bar{x}_1-\bar{x}_2)-\mu}{\sqrt{\frac{s^2_{\bar{x}_1}}{n_1}+\frac{s^2_{\bar{x}_2}}{n_2}}}$ | $n_1+n_2-2$                                                                                                                                                                        | Independent groups and same constant true variance                       |
| Welch's t-test              | $\frac{(\bar{x}_1-\bar{x}_2)-\mu}{\sqrt{\frac{s^2_{\bar{x}_1}}{n_1}+\frac{s^2_{\bar{x}_2}}{n_2}}}$ | $\approx \frac{(\frac{s^2_{\bar{x}_1}}{n_1}+\frac{s^2_{\bar{x}_2}}{n_2})^2}{\frac{(\frac{s^2_{\bar{x}_1}}{n_1})^2}{n_1-1}+\frac{(\frac{s^2_{\bar{x}_2}}{n_2})^2}{n_2-1}}$, rounded | Independent groups and unequal constant variance. Both group samples > 5 |
| Paired t-test               | $\frac{\bar{d}-d_\mu}{\frac{s_{\bar{d}}}{\sqrt{n}}}$                                               | n-1                                                                                                                                                                                | Pairings between groups                                                  |


Welch's t-test will give a larger p-value compared to 2 sample t-test
- Welch's df approximation will tend to give a smaller df -> larger tails -> larger p-values
- This means it is less likely to reject the null hypothesis
# Derivation



# Related
- These are the parametric analog to the [[Wilcoxon Rank Test]]
