---
tags:
---

# Definition
A transformation is a function on a random variable
This changes the outcomes and thus the distribution


# Methods


## Method of CDF
We find the distribution by finding the cdf to get the pdf. The pdf identifies the distribution

Must be a monotone transformation because we want a [[one to one]] mapping

let X be a random variable, g(X) be a transformation on X
$$
\begin{aligned}
F_{g(X)}(c) &= P(g(X)<c)\\
&=P(X<g^{-1}(c))\\
\frac{\partial}{\partial c}F_{g(X)}(c) &=f_{X}(g^{-1}(c))|\frac{\partial g^{-1}(c)}{\partial c}|\\ 
\end{aligned}
$$




Expanding this to a series of equations

$$
\begin{aligned}
Y_1=g_1(X_1,X_2,X_3)\\
Y_2=g_2(X_1,X_2,X_3)\\
Y_3=g_3(X_1,X_2,X_3)\\
f(Y_1,Y_2,Y_{3})= f(X_1=h_1(Y_1,Y_2,Y_3),\\X_2=h_2(Y_1,Y_2,Y_3),\\X_3=h_3(Y_1,Y_2,Y_3))|J|\\
J_1=
\begin{vmatrix} 
\frac{\partial g_1}{\partial X_{1}}  & \frac{\partial g_2}{\partial X_{1}}& \frac{\partial g_3}{\partial X_1} \\ 
\frac{\partial g_1}{\partial X_{2}}& \frac{\partial g_2}{\partial X_{2}}& \frac{\partial g_3}{\partial X_{2}} \\ 
\frac{\partial g_1}{\partial X_{3}}& \frac{\partial g_2}{\partial X_{3}}& \frac{\partial g_3}{\partial X_3}
\end{vmatrix}\\
J_{2}=
\begin{vmatrix} 
\frac{\partial h_1}{\partial Y_{1}}  & \frac{\partial h_2}{\partial Y_{1}}& \frac{\partial h_3}{\partial Y_1} \\ 
\frac{\partial h_1}{\partial Y_{2}}& \frac{\partial h_2}{\partial Y_{2}}& \frac{\partial h_3}{\partial Y_{2}} \\ 
\frac{\partial h_1}{\partial Y_{3}}& \frac{\partial h_2}{\partial Y_{3}}& \frac{\partial h_3}{\partial Y_3}
\end{vmatrix}\\
\end{aligned}
$$
We multiply $|\frac{1}{J_1}|$ for the input jacobian, $|J_2|$ for the output [[Jacobian Matrix]], which ever is easier

If the transformation is not 1 to 1, we break up the intervals so it becomes 1 to 1, summing them all up

Get joint pdf -> get Jacobian -> substitute -> observe if joint is separable

## [[Moment Generating Function]]
Easiest with linear transformations
$$
\begin{align}
M_{aX+b}(t) &=E(e^{t(aX+b)})\\
&=e^{tb}E(e^{atX})\\
&= e^{tb}M_X(at)
\end{align}
$$


# Side notes
If the transformation is the cdf of the RV, then it transforms into uniform(0,1)

Ex.
$$
\begin{aligned}
X\sim exp(\lambda)\\
Y = 1-e^{-\lambda X}\\
\implies Y \sim U(0,1)
\end{aligned}
$$

