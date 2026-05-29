---
tags:
  - Statistics/Theory
  - Statistics/Models/Linear
---

# Definition
Simple [[Linear Regression]] can be seen as a projection of the response to the space of predictors

That is to say, we have a vector space composed of the predictors and 1's as basis vectors.
- The response may be within this span
- The error vector is the perpendicular from the span to the response 
	- A good model means this will be small
- $\vec{\hat{y}}$ is a projection of $\vec{y}$ onto the $span\{\vec{1},\vec{x}\}$


![[orthogonal projection.png]]
# Notes

## Orthogonal Basis
$\vec{1}$ is not orthogonal to $\vec{x}$, so we can use the [[Gram-Schmidt Process]] to create an orthogonal basis.

This creates a vector space derived from the data

## Predictors are orthogonal to the errors
Intuitively, the errors are a vector from the our predictor basis

The result is that $\vec{e}\perp \vec{x}$ because that minimizes the distance from the $span\{\vec{1},\vec{x}\}$ and response. 
- We are not working in curved space because of linearity

# Related
- [Orthogonal Projection Formulas (Least Squares) - Projection, Part 2](https://www.youtube.com/watch?v=73xKLFsXvvM)
![[orthogonal projection.png]]

