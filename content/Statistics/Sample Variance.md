---
tags:
  - Statistics/Theory
---

# Definition
The sample variance is a [[Random Variable]] that is a function of the data.
$$
\begin{aligned}
x_i &\sim Normal(\mu,\sigma^2)\\
\implies \sum^n_{i=1} (\frac{x_i-\mu}{\sigma})^2 &\sim \chi^2_{n}\\
s^2 &= \sum^n_{i=1} (\frac{(x_i-\mu)^2}{n-1})\\
(n-1)s^2 &= \sum^n_{i=1} (x_i-\mu)^2\\
\frac{(n-1)s^2}{\sigma^2} &= \sum^n_{i=1} (\frac{x_i-\mu}{\sigma})^2\\
\implies \frac{(n-1)s^2}{\sigma^2} &\sim \chi^2
\end{aligned}
$$

There are a few estimators that can be used as the sample variance.

## Unbiased Estimator
$$
\begin{aligned}
s^2 &= \frac{\sum^n_{i=1}(x_i-\bar{x})^2}{n-1}\\
E(s^2) &= E(\frac{\sum^n_{i=1}(x_i-\bar{x})^2}{n-1})\\
&= \frac{1}{n-1}\sum^n_{i=1}E((x_i-\bar{x})^2)\\
(x_i-\bar{x})^2 &= (x_i-\mu+\mu-\bar{x})^2\\
&= (x_i-\mu)^2+(\mu-\bar{x})^2 - 2 (x_i-\mu)(\mu-\bar{x})\\
E((x_i-\bar{x})^2) &=  E((x_i-\mu)^2+(\mu-\bar{x})^2 - 2 (x_i-\mu)(\mu-\bar{x}))\\
&= var(x_i) + var(\bar{x}) - 2E((x_i-\mu)(\mu-\bar{x}))\\
&= \sigma^2 + \frac{\sigma^2}{n} - 2E((x_i-\mu)(\mu-\bar{x}))\\
E((x_i-\mu)(\mu-\bar{x})) &= E(x_i\mu - x_i\bar{x} - \mu^2+\mu\bar{x})\\
&= \mu\mu - E(x_i\bar{x}) - \mu^2 + \mu E(\bar{x})\\
&= \mu^2 - E(x_i \frac{\sum^n_{j=1} x_j}{n}) \\
&= \mu^2-\frac{1}{n}E(x_i^2 + \sum_{j\neq i} x_ix_j)\\
&= \mu^2 - \frac{1}{n}[(var(x_i)+\mu^2) + (n-1)\mu\mu]\\
&= \mu^2 - \frac{\sigma^2}{n}-\frac{\mu^2}{n} - \frac{n-1}{n}\mu^2\\
&= \frac{\sigma^2}{n}\\
E((x_i-\bar{x})^2) &= \sigma^2+\frac{\sigma^2}{n}-2\frac{\sigma^2}{n}\\
&= \frac{n-1}{n}\sigma^2\\
E(s^2) &= \frac{1}{n-1}\sum^n_{i=1} [\frac{n-1}{n}\sigma^2]\\
&= \sigma^2
\end{aligned}
$$

The $\frac{n-1}{n}$ factor in this estimator is known as [[Bessel's Correction]] and it is due to using the [[Sample Mean]] as part of estimating the variance. This removes one degree of freedom.

## MLE Estimator

$$
\begin{aligned}
s^2 = \frac{\sum^n_{i=1}(x_i-\bar{x})^2}{n}
\end{aligned}
$$



