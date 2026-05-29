---
tags:
  - Linguistics
  - Computer-Science
---

# Definition
A distance metric between strings that measures how many edits it takes to go from one word to another.


# Algorithm
$$
\begin{aligned}
lev(a,b) = 
\begin{cases}
|a| & if |b|=0,\\
|b| & if |a|=0,\\
lev(tail(a), tail(b)) & if head(a)=head(b),\\
1+min
\begin{cases}
lev(tail(a),b)\\
lev(a,tail(b))\\
lev(tail(a),tail(b))
\end{cases}
& otherwise
\end{cases}
\end{aligned}
$$


# Related
- [[Hamming Distance]]

