---
tags:
  - Statistics/Theory
---
# Definition
A set of distributions that fit the form of:
$$
f(x|\vec{\theta})=h(x)c(\vec{\theta})exp(\sum\limits^k_{i=1}w_i(\vec{\theta})t_i(x))
$$
basically, $f(x|\vec{\theta})$ = f(only x)c(only theta) exp(sum of w(only theta)* t(only x))

# Theorems
$$
\begin{aligned}
E[\sum\limits^{k}_{i=1}\frac{\partial w_i(\vec{\theta})}{\partial\theta_j}t_{i}(x)]&= -\frac{\partial}{\partial\theta_{j}}ln(c(\vec{\theta}))\\
var[\sum\limits^{k}_{i=1}\frac{\partial w_i(\vec{\theta})}{\partial\theta_j}t_{i}(x)]&= -\frac{\partial^2}{\partial\theta_{j}^2}ln(c(\vec{\theta}))-E[\sum\limits^{k}_{i=1}\frac{\partial^2 w_i(\vec{\theta})}{\partial\theta_j^2}t_{i}(x)]\\
\end{aligned}
$$
Note the left hand side uses the exponentiated functions


# Related

