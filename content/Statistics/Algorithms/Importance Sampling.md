---
tags:
  - Algorithms
---
# Definition
An algorithm used to estimate an integral $I=\int^{b}_{a}h(x)dx$

# Variations

## Monte Carlo Integration

```
1. Let X = array of n elements sampled iid Uniform(a,b)
2. Let h_X = array of n elements, each being h(X_i) for all X
3. h_bar = avg(h_X)
4. Estimator = (b-a)*h_bar
```

The sample mean (integral estimator) will converge to the true mean (true integral value) as an unbiased estimator
The variance of the sample mean is $Var(\frac{b-a}{n}var(\bar{h}))=\frac{(b-a)^2}{n}Var(h(x))$

We are considering each h(x) equally as each have equal weights
The issue is that we could waste time on computing **unhelpful** values

Issues:
- Each h(x) value are weighed equally. This can hold back the average
- Need to know the distribution (be able to sample directly) 
## Importance sampling
This overcomes the struggles of being unable to sample directly by adding ideas from rejection sampling: We reject values if they "dont make sense"

We turn this as a weighted average where the weights depend on the true distribution (f) and simple distribution (g)

```
1. Let X = array of n elements sampled iid Uniform(a,b)
2. Let h_X = array of n elements, each being h(X_i) for all X
3. Let f_X = array of n elements from true distribution 
4. Let g_X = array of n elements, each being g(X_i) for all X
5. f_g = ratio of f(x_i)/g(x_i) # these are the weights
6. h_bar = (f_g dot h(x))/n # weighted average of h(x)
7. Estimator = (b-a)*h_bar
```


# Math

$$
\begin{aligned}
\text{Importance sampling}\\
E_{f[h(X)]}&= \int_{D}h(x)f(x)dx\\
&= \int_Dh(x)\frac{f(x)}{g(x)}g(x)dx\\
&= E_{g}[h(X)\frac{f(x)}{g(x)}]\\
\end{aligned}
$$

# Related
