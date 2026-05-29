

# Definition
A method of direct differentiation using [[Dual Numbers]]

$$
\begin{aligned}
f(x+\epsilon) = 
\end{aligned}
$$


## Examples


### Polynomial
$$
\begin{aligned}
f(x) &= x^n\\
f(x+\epsilon) &= (x+\epsilon)^n\\
&= x^n + nx^{n-1}\epsilon + O(\epsilon^2)\\
&= f(x) + f'(x)\epsilon
\end{aligned}
$$

### Exponential
$$
\begin{aligned}
f(x) &= ae^{bx}\\
&= a\sum^\infty_{n=0} \frac{(bx)^n}{n!}\\
f(x+\epsilon)&=ae^{b(x+\epsilon)}\\
&= ae^{b\epsilon} e^{bx}\\
&= (\sum^\infty_{n=0} \frac{(b\epsilon)^n}{n!})f(x)\\
&= (\frac{(b\epsilon)^0}{0!} + \frac{(b\epsilon)^1}{1!})f(x)\\
&= f(x) + f'(x)\epsilon\\
\end{aligned}
$$



