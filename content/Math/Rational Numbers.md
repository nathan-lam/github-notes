---
tags:
  - Mathematics/Objects
---

# Definition
A number that can be expressed as the ratio of two [[Integer Numbers]] where the denominator cannot be zero.

The important things to note are:
- The order of the integer numbers matter
- The denominator cannot be zero
- two distinct ratios are the same if they can simplify the sameway
	- The precise way is to cross multiply them
## Exact definition
$$
\mathbb{Q}=\{\frac{p}{q}: p,q\in\mathbb{Z}, q\neq0\}
$$
This set is precisely described as an ordered pair in $\mathbb{Z}\times\mathbb{Z}_{/\{0\}}$ with the [[Equivalence Relations]]: $(p,q) \sim (m,n)$ if $pn=mq$ and $q\neq0\neq n$
- This helps relate similar ratios together, like 1/2 = 2/4
- It is a valid equivalence relation because it satisfies the conditions
	- Reflexivity
		- $(p,q)\sim(p,q) \implies pq = pq$ is true
	- Symmetric
		- $(m,n) \sim (p,q) \implies mq=pn$ is true
	- Transitivity
		- $(p,q) \sim (m,n) \text{ and } (m,n)\sim (a,b) \implies (p,q) \sim (a,b)$
		- pn=mq and mb = an to show pb = aq 
		- $b(pn) = b(mq) \implies n(pb)=b(mq)=(mb)q = (an)q, n\neq0 \land n(pb) = n(aq) \implies pb=aq$

The ordered pairs are such that there is an [[Isomorphic|isomorphism]] between $\frac{n}{1}\in\mathbb{Q}$ and $n\in\mathbb{Z}$
- This is to say that the integers are contained in the rationals, $\mathbb{Z}\subset\mathbb{Q}$


This helps define what addition is for the rationals
- adding with 1/2 or 2/4 should give the same result
	- $\frac{a}{b}+\frac{c}{d} = \frac{a+c}{b+d}$ gives different results depending on the representation
		- $\frac{1}{2} + \frac{1}{3} \neq \frac{2}{4}+\frac{1}{3}$ under this definition of addition
		- This is not [[Well Defined]]


# Properties


## Addition
Addition between two fractions is defined as
$$\frac{a}{b} + \frac{c}{d} = \frac{ad+bc}{bd}$$
- This is well defined
	- if (a,b) ~ (a',b') and (c,d) ~ (c',d')
		-  (a,b) ~ (a',b') -> ab' = a'b
		- (c,d) ~ (c',d') -> cd' = c'd
		- (a,b) + (c,d) = (ad+bc, bd)
		- (a',b') + (c',d') = (a'd'+b'c', b'd')
		- (ad+bc, bd) ?~ (a'd'+b'c', b'd')
			- (ad+bc) * b'd' = (a'd'+b'c') * (bd)
			- adb'd' + bcb'd' = bda'd' + bdb'c'
			- adb'd' + bcb'd' = (ab')(dd') + (bb')(cd'), which is true
			- therefore this is well defined

## Multiplication
Multiplication between two fractions is defined as
$$\frac{a}{b} \cdot \frac{c}{d} = \frac{ac}{bd}$$


## [[Ordering]]


