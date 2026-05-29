---
tags:
  - Mathematics/Calculus
  - Mathematics/Proofs
---

# Definition
The formal definition of a limit, $\lim_{x\to c} f(x) = L$

# Explanation

The key idea is that the output is within a tolerance level when the input is withing a tolerance level
$$
\begin{aligned}
\text{A limit exists,}\lim_{x\to c} f(x) = L, \\
\forall\epsilon>0 , \exists \delta>0 \text{ such that }\\
\forall x\neq c, 0<|x-c|<\delta \implies |f(x)-L|<\epsilon\\
\end{aligned}
$$

In english: 
- A limit of a function, $f(x)$, with an input approaching c means we can have an input tolerance that implies an output tolerance.
- If there is a limit, then we can always find the input tolerance ($\delta$) that gets the output tolerance ($\epsilon$) close to $L$

$\delta$ is a positive wiggle in x that implies f(x) has a wiggle of positive wiggle $\epsilon$

The point is that $\delta, \epsilon$ can be arbitrarily small (but not zero) to say that a function approaches a value.
- Once $\delta=0= \epsilon$ then that is the exact value
- Recall that an output may not exist in a function, but the function can still approach the value.
	- $\frac{x^2-1}{x-1}$ does not exist at x=1, but the limit still approaches 2


# Example
To prove a limit exists, you need to assert $\exists \epsilon>0$ and find what $\delta>0$ makes the statement $0<|f(x)-L|<\epsilon$ true

## $\lim_{x\to 4}\sqrt{2x+1}$


Doing some algebra we can find what $\delta$ should be
$$
\begin{aligned}
|\sqrt{2x+1}-3| &= |\frac{(\sqrt{2x+1}-3)(\sqrt{2x+1}+3)}{\sqrt{2x+1}+3}|\\
&= |\frac{(2x+1)-3^2}{\sqrt{2x+1}+3}|\\
&= |\frac{2(x-4)}{\sqrt{2x+1}+3}|\\
\sqrt{2x+1}+3 > 1 \implies |\sqrt{2x+1}-3|=|\frac{2(x-4)}{\sqrt{2x+1}+3}|&< |2(x-4)|\\
\text{suppose } 0<|x-4|<\delta \implies |\sqrt{2x+1}-3| < 2|x-4|&< 2\delta\\
|\sqrt{2x+1}-3| < \epsilon \implies \delta=\frac{\epsilon}{2}\\
\end{aligned}
$$


Putting it all together
$$
\begin{aligned}
\text{To prove }\lim_{x\to 4}\sqrt{2x+1} = 3\\
\text{There needs to exist } \epsilon>0,\delta>0, s.t.\\
0<|x-4|<\delta\implies |\sqrt{2x+1}-3|<\epsilon\\
\text{This is found with the existence of } \delta=\frac{\epsilon}{2}
\end{aligned}
$$
If we cannot find $\delta$, then the limit does not exist

# Related
- [# epsilon-delta definition ultimate introduction](https://www.youtube.com/watch?v=DdtEQk_DHQs)
- [Limits, L'Hôpital's rule, and epsilon delta definitions | Chapter 7, Essence of calculus](https://www.youtube.com/watch?v=kfF40MiS7zA)]
- [LibreTexts Mathematics](https://math.libretexts.org/Bookshelves/Calculus/Calculus_3e_(Apex)/01%3A_Limits/1.02%3A_Epsilon-Delta_Definition_of_a_Limit)

