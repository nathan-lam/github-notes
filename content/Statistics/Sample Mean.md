---
tags:
  - Statistics/Theory
---

# Definition
The sample mean is a [[Random Variable]] that is a function of the data, $$\bar{X} = \frac{1}{n}(X_1+X_2+\dots+X_n)$$

Assuming that each sample is [[Independent and Identically Distributed]], then $\bar{X}$ converges to the [[Normal]] distribution no matter the distribution of $X_i$. This is the [[Central Limit Theorem]].


$$
\begin{aligned}
E(\bar{X}) &= E(\frac{1}{n}\sum^n_{i=1}X_i)\\
&= \frac{1}{n}\sum^n_{i=1}E(X_i)\\
&= \frac{1}{n}(n\mu), X_i\text{ are }iid\\
&= \mu\\
var(\bar{X}) &= var(\frac{1}{n}\sum^n_{i=1}X_i)\\
&= \frac{1}{n^2}\sum^n_{i=1}var(X_i), X_i\text{ are }iid\\
&= \frac{1}{n^2}(n\sigma^2)\\
&= \frac{\sigma^2}{n}\\
\lim_{n\to\infty} \bar{X} &\sim Normal(\mu,\frac{\sigma^2}{n})\\
\therefore \frac{\bar{X}-\mu}{\sqrt{\frac{\sigma^2}{n}}} &\sim Normal(0,1)\\
\end{aligned}
$$


# Related
- Averaging reduces variance



