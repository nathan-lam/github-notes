---
knowledge_classes:
  - UCB-stat154
  - UCLA-stat413
tags:
  - Statistics/Theory
---
The Neural network component that allows to achieve nonlinearity



| Name    | f(x)                                | f'(x)           |
| ------- | ----------------------------------- | --------------- |
| Linear  | x                                   | 1               |
| ReLU    | $max(0, x)$                         | 1 if x>0 else 0 |
| Sigmoid | $\frac{1}{1+e^{-x}}$                | $f(x)(1-f(x))$  |
| tanh    | $\frac{e^{x}-e^{-x}}{e^{x}+e^{-x}}$ | $1-f^2(x)$      |
|         |                                     |                 |

Softmax is also an activation function but operates elementwise
it's the multivariate version of the sigmoid

