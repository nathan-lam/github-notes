---
tags:
  - Mathematics/Derivations
---


# Claim
The dot product is a measure of how [[Orthogonal|orthogonal]] two vectors are.


# Derivation
Two vectors can be seen as two edges of a triangle with the difference vector acting as the third edge.
By using the [[Law of Cosine]], it can be shown directly that the dot product relates to the angle of the two vectors.
$$
\begin{aligned}
&\text{Let } \vec{u}, \vec{v} \text{ be arbitrary vectors}\\
\theta &:= \text{ Angle between }\vec{u}, \vec{v}\\
&\text{A triangle can be formed with side lengths }||\vec{u}||, ||\vec{v}||, ||\vec{u}-\vec{v}||\\
||\vec{u}-\vec{v}||^2 &= ||\vec{u}||^2+||\vec{v}||^2-2||\vec{u}||||\vec{v}||\cos\theta, \text{Law of Cosine}\\
||\vec{u}-\vec{v}||^2 &= (\vec{u}-\vec{v})\cdot (\vec{u}-\vec{v})\\
&=||\vec{u}||^2+||\vec{v}||^2-2(\vec{u}\cdot\vec{v})\\
||\vec{u}||^2+||\vec{v}||^2-2(\vec{u}\cdot\vec{v}) &= ||\vec{u}||^2+||\vec{v}||^2-2||\vec{u}||||\vec{v}||\cos\theta\\
\vec{u}\cdot\vec{v} &= ||\vec{u}||||\vec{v}||\cos\theta\\
&\therefore \text{The dot product is a measure of orthogonality}\\
\end{aligned}
$$

# Related
- [Cosine Formula for Dot Product](https://proofwiki.org/wiki/Cosine_Formula_for_Dot_Product)
