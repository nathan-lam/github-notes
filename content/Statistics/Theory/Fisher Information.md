---
tags:
  - Statistics/Theory
---

# Definition
The amount of information of a random variable based on a parameter $\theta$

The fisher information has several ways to compute the quantity
$$
\begin{aligned}
\mathit{I}(\theta) &= E_\theta[(\frac{\partial}{\partial\theta} \log f(X;\theta))^2]\\
&= Var_\theta[\frac{\partial}{\partial\theta} \log f(X;\theta)]\\
&= -E_\theta[\frac{\partial^2}{\partial\theta^2}\log f(X;\theta)]\\
\end{aligned}
$$
where $\log f(X;\theta)$ is the log likelihood function

## Multivariable Definition
The definition above is for single variable, but it is possible to extend the fisher information from a single value to a matrix.
$$
\begin{aligned}
\mathit{I}(\theta)_{ij} &= Cov_\theta[\frac{\partial}{\partial\theta_i} \log f(X;\theta), \frac{\partial}{\partial\theta_j} \log f(X;\theta)]\\

&= -E_\theta[\frac{\partial^2}{\partial\theta_i\theta_j}\log f(X;\theta)]\\
\end{aligned}
$$

# Asymptotic Distribution
If a sample is [[Independent and Identically Distributed|iid]], then the sample estimate has an [[Asymptotic Distributions|asymptotic distribution]] of
$$\lim_{n\to\infty} \frac{(\hat{\theta}_n)-\theta}{\frac{1}{\sqrt{n \mathit{I}(\theta)}}} \sim Normal(0,1)$$



# Related
- https://arxiv.org/pdf/1705.01064
- 

