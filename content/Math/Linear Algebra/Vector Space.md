---
tags:
  - Mathematics/Linear-Algebra
---

# Definition

A vector space is a set that has the following properties
- Operates under finite vector addition and scalar multiplication

Vector operations has the following properties
$$
\begin{aligned}
\text{Associative under vector addition}& & \vec{u} +(\vec{v}+\vec{w}) &= (\vec{u}+\vec{v})+\vec{w}\\
\text{Communtative under vector addition}& & \vec{u} + \vec{v} &= \vec{v} + \vec{u}\\
\text{Distributive under vector addition}& & r(\vec{u}+\vec{v}) &= r\vec{u} + r\vec{v}\\
\text{Identity element for vector addition}& & \vec{0} + \vec{v} &= \vec{v}\\
\text{Inverse element for vector addition}& & \vec{v} + (-\vec{v}) &= \vec{0}\\
\end{aligned}
$$
Scalar operations has the following properties
$$
\begin{aligned}
\text{Associative under scalar multiplication}& & r(s\vec{v}) &= (rs)\vec{v}\\
\text{Distributive under scalar multiplication}& & (r+s)\vec{v} &= r\vec{v} + s\vec{v}\\
\text{Identity element for scalar multiplication}& & 1\vec{v} &= v\\

\end{aligned}
$$


Vector spaces typically have a method to measure distance, but it not a necessary condition.
- [[Norm]] is the measured length of a vector
- [[Inner Product]] is the measured distance between vectors
	- Can imply a norm if taking the inner product of a vector with itself


# Related
- Polynomial Vector Space
	- [[Legendre Polynomials]]
	- [[Chebyshev Polynomials]]
- [[Differential Equations]]
