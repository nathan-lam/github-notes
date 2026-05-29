---
tags:
---

# Definition
A Fourier Series is a sinusoidal representation of any function which can be written as the following

$$
f(x) = \frac{A_0}{2} + \sum^{\infty}_{k=1}( A_k\cos(kx) + B_k\sin(kx))
$$
We want to find a what coefficients to get this representation

# How to get the Coefficients

We get this coefficients by getting the [[Inner Product]] of the target function and basis functions
$$
\begin{aligned}
A_k = \frac{1}{L}\int^{\pi}_{-\pi} f(x) \cos(kx)dx
B_k = \frac{1}{L}\int^{\pi}_{-\pi} f(x) \sin(kx)dx
\end{aligned}
$$

