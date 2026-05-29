---
tags:
  - Statistics/Inference
---

# Definition
The probability of observing the data (or greater) assuming the null hypothesis is true.

Depending on how the hypothesis is set up, the p value can be:
$$
\begin{aligned}
P(T \geq t | H_0) &= \text{P-Value of a right one tail statistic}\\
P(T \leq t | H_0) &= \text{P-Value of a left one tail statistic}\\
2 min(P(T \geq t | H_0), P(T \leq t | H_0)) &= \text{P-Value of a two tail statistic}
\end{aligned}
$$

Do note that we include the extreme ends as that gives a benefit of a doubt to the hypothesis.


If the p-value is less than the critical value, then we reject the null hypothesis. 
- "We reject the null hypothesis"

Otherwise, we accept the null
- "We failed to reject the null hypothesis"
- This does not mean that the null hypothesis is correct, but that the evidence does not support the alternative theory.
# Warnings
The p-value is an abstract concept and is prone to misunderstandings.


## P-values as a statement about the hypothesis
The p-value does not state whether the null or alternative is true or not.

It is a statement "If X were" true, then it is reasonable to measure the data like what was observed.

A hypothesis could be that the data was produce by random chance, but this is not the default.
- The hypothesis is a defined model, which could be random chance.

## Measure of correctness.
The magnitude of the p-value does not indicate a strength in correctness. 

A p-value = 0.01 or 0.001 does not mean the latter has a stronger hypothesis.

The p-value is a statement of likelihood of the data

## [[P-Hacking]]
An unethical approach to find statistically significant results.

It is possible for an experiment to give a statistically significant result when there is none. 
- This is made worse when test among a variety of groups, one is bound to be significant.

If testing many groups, the p-value needs to be adjusted.
- ???-tukey test
- [[Bonferroni Correction]]

# Related
- 