---
tags:
  - Mathematics/Linear-Algebra
---

# Definition
An operation that measures the relationship between two vectors

It takes two vectors and outputs a real number
- $\langle \cdot, \cdot \rangle: \vec{v}\times\vec{v} \rightarrow \mathbb{R}$

A inner product is defined with the following properties
$$
\begin{aligned}
\text{Strictly non-negative}&& &\langle\vec{v},\vec{v}\rangle \geq 0, &\langle\vec{v},\vec{v}\rangle = 0 \iff \vec{v}=\vec{0}\\
\text{Linearity with left argument} && &\langle\vec{u}+\vec{v},\vec{w}\rangle = \langle\vec{u},\vec{w}\rangle +\langle\vec{v},\vec{w}\rangle\\
\text{Conjugate symmetry} && &\langle\vec{u},\vec{v}\rangle = \overline{\langle\vec{v}, \vec{u}\rangle}
\end{aligned}
$$

# Related
- [[Norm]]
- [[Dot Product]]

