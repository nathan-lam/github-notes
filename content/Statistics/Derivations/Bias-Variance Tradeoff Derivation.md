


$$
\begin{aligned}
\text{Mean Squared Error} &= MSE(\hat{\theta}) = E([y - f(x|\hat{\theta})]^2)\\
y=f(x|\theta)+\epsilon &=\text{true values = true model + noise}, \\
\text{noise} = \epsilon &\sim N(0,\sigma^2)\\
f(x|\hat{\theta}) &= \text{model of y using x with parameter }\hat{\theta}\\
E([y - f(x|\hat{\theta})]^2) & = E([f(x|\theta)+\epsilon - f(x|\hat{\theta})]^2), &y=f(x|\theta)+\epsilon\\
&=E([f(x|\theta) - f(x|\hat{\theta})]^2 + 2[f(x|\theta) - f(x|\hat{\theta})]\epsilon + \epsilon^2), &\text{foil } (a+b)^2: a= f(x|\theta) - f(x|\hat{\theta}), b = \epsilon\\
&=E([f(x|\theta) - f(x|\hat{\theta})]^2) + 2E([f(x|\theta) - f(x|\hat{\theta})]\epsilon) + E(\epsilon^2), &\text{Linearity property of expectation}\\
&=E([f(x|\theta) - f(x|\hat{\theta})]^2) + 0 + E(\epsilon^2), &\epsilon\perp x \implies \text{Can pull out }E(\epsilon)=0\\
&=E([f(x|\theta) - f(x|\hat{\theta})]^2)  + \sigma^2, & E(\epsilon^2) = \sigma^2\\
E([f(x|\theta) - f(x|\hat{\theta})]^2) &= E([f(x|\theta) - E(f(x|\hat{\theta})) + E(f(x|\hat{\theta}))) + f(x|\hat{\theta})]^2), &E(f(x|\hat{\theta})) - E(f(x|\hat{\theta}))) = 0\\
&= E([f(x|\theta) - E(f(x|\hat{\theta}))]^2)
\end{aligned}
$$



