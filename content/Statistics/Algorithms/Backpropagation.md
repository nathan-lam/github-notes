---
tags:
  - Statistics/Theory
---
The technique used to fit all [[Neural Networks]]

This is ultimately stacked chain rule
- As we go deeper into the network, the more partial derivatives have to be calculated

$$
\begin{aligned}
\frac{d}{dx}f(g(x))&= \frac{df}{dg}\frac{dg}{dx}\\
\frac{d}{dx}f(g(h(x)))&= \frac{df}{dg}\frac{dg}{dh}\frac{dh}{dx}
\end{aligned}
$$



It is possible to vectorize backpropagation, but some rearrangement is needed as the dimensions wont fit

