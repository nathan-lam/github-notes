---
tags:
  - Mathematics
---

# Defintion

An infinite sequence of numbers encoded as the coefficients of a single function.


We can encode the sequence $a_0, a_1, a_2, \dots$ as the coefficients like below: 
$$
\begin{aligned}
\sum^\infty_{n=0} a_n\cdot x^n  
\end{aligned}
$$

# Example

Encoding the natural numbers
$$
\begin{aligned}
\text{let }a_n &= n\\
\implies S(x) = \sum^\infty_{n=0} n\cdot x^n &= 0\cdot x^0 + 1\cdot x^1 + 2\cdot x^2 + \dots \\
&= x \sum^\infty_{n=0} n\cdot x^{n-1}\\
&= x \frac{d}{dx}(\sum^\infty_{n=0} x^{n})\\
&= x \frac{d}{dx} \frac{1}{1-x}\\
&= x \frac{1}{(1-x)^2}\\
&= \frac{x}{(1-x)^2}\\
\therefore S(x) &= \frac{x}{(1-x)^2}\\
S(x) &\text{ encodes all natural numbers}
\end{aligned}
$$
To get the sequence back, create the taylor series of the function and read off the coefficients.

# Related
- This is the same tool for [[Moment Generating Function]]
	- note the minor difference that the MGF can extract terms by using the nth derivative an evaluating at 0 while generating functions do not do this as a default.

