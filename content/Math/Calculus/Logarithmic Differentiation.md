---
tags:
  - Mathematics/Calculus
---

# Definition
A trick to get a derivative


# Example

$$
\begin{aligned}
f(x) &= x^x\\
\log(f(x)) &= log(x^x)\\
&= xlog(x)\\
\frac{d}{dx} \log(f(x)) =  \frac{f'(x)}{f(x)} &= \frac{d}{dx}  xlog(x)\\
&= log(x) + x(\frac{1}{x})\\
&= log(x)+1\\
\implies f'(x) &= f(x)\cdot (log(x)+1)\\
&= x^x(log(x)+1)
\end{aligned}
$$

