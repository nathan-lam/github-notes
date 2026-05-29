---
tags:
  - Mathematics/Calculus
---

# Definition
A technique to help break up an integral.

$$
\int u(x)v(x)dx = u(x) \cdot \int v(x)dx - \int u'(x)\cdot[\int v(x) dx]dx
$$

The rule of thumb for picking the u function:
1. Log
2. Inverse trig
3. Algebraic
4. Trig
5. Exp



# Example
$$
\begin{aligned}
\int^{\pi/2}_0 x \cos x dx\\
\text{Let }u = x, v = \cos x\\
\int^{\pi/2}_0 x \cos x dx &= x|^{x=\pi/2}_{x=0} \int^{\pi/2}_0\cos xdx - \int^{\pi/2}_0 1\cdot [\int \cos x dx]dx\\
&= \frac{\pi}{2}(\sin x|^{x=\pi/2}_{x=0}) - \int^{\pi/2}_0 \sin x dx\\
&=  \frac{\pi}{2}\cdot 1 - (-\cos x|^{x=\pi/2}_{x=0}) \\
&=  \frac{\pi}{2} -1
\end{aligned}
$$


# Derivation
This is derived by the product rule of derivatives:
$$
\begin{aligned}
\text{Product rule: }\frac{d}{dx}u(x)v(x) = u'(x)v(x) + u(x)v'(x)\\
\int [\frac{d}{dx}u(x)v(x) = u'(x)v(x) + u(x)v'(x)], \text{Integrate both sides}\\
u(x)v(x) = \int u'(x)v(x)dx + \int u(x)v'(x)dx\\
\int u(x)v'(x)dx = u(x)v(x) - \int u'(x)v(x)dx
\end{aligned}
$$




# Related
- 

