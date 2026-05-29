---
tags:
  - Mathematics/Theorems
---

# Definition
A condition that allows for summation and integration to be interchanged.

$$
\begin{aligned}
&\text{if }\sum^\infty_{n=0} f_n(x) \text{ exists for all }x \text{ AND there exists integrable function }g(x) \text{ such that } |\sum^\infty_{n=0} f_n(x)|\leq g(x) \forall k\\
&\text{then }\int\sum^\infty_{n=0} f_n(x)dx = \sum^\infty_{n=0} \int f_n(x)dx
\end{aligned}
$$

# Notes
The triangle inequality can be used as a choice g(x) 
- $|\sum a_n | \leq \sum |a_n| \implies g(x) = \sum^\infty_{n=0} |f_n(x)|$
- g(x) also becomes a test of [[Absolute Convergence]] if g(x) converges

# Related
- https://www.youtube.com/watch?v=N-e5MJ3tHOk


