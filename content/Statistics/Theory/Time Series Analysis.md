---
tags:
  - Statistics/Applications
---

An area of application that focuses on data trending across time


# Methods
Goal: to predict the future
- Done by striving for [[Stationary]]

We model the data until we achieve [[Stationary#White Noise]]

Model signal + noise = (tend + seasonality) + Noise


# Signal Modelling
Any model is viable
- Linear Regression is common
- Add sinusoidal terms for seasonality
- Differencing
	- Analogous to a derivative operator so we difference until we see no more trend


# Noise Modelling
- based on previous terms [[Auto Regressive Model]] 
- based on white noise terms [[Algorithm - MA]]

Ex. ARMA(2,3)
$$\begin{aligned}
X_{10} &= \phi_{1}X_{9}+ \phi_{2}X_{8} + \omega_{10}+\theta_{1}\omega_{9}+\theta_{2}\omega_{8}+\theta_{3}\omega_{7}\\
(1-\phi_{1}B- \phi_{2}B^2)X_{10}&=(1+\theta_{1}B+\theta_{2}B^2+\theta_{3}B^3)\omega_{10}\\
\hat{X}_{10} &= \phi_{1}X_{9}+ \phi_{2}X_{8} + \theta_{1}\omega_{9}+\theta_{2}\omega_{8}+\theta_{3}\omega_{7}
\end{aligned}$$
Notice that each side has a polynomial, if they share a common term, this obscures the actual patterns

## Diagnosing Noise models


Count the number of lags that stick pas the confidence interval (ignoring lag 0)
- [[ACF Plot]] - Helps find MA(q)
- [[PACF Plot]] - Helps find AR(p)
Then compare with theoretical plot based on the model decided


MA models could be non unique if not invertible



# Properties

## Invertibility
A condition where an MA(q) model, $X_{t}=\Theta(B)W_{t}$,, with the roots of $\Theta(B)$ polynomial being greater than 1
|polynomial roots| > 1 iff |MA coef| < 1

This implies a **unique** solution

Says that current white noise is composed all previous measurements
All AR models are invertible

## Causality
Indicates that there is a **causal** relationship from the past to the future 
|polynomial roots| > 1 iff |AR coef| < 1

Says that current measurement is composed of all previous white noise
All MA models are causal


# Rule of thumbs
Dont remove data points, especially in the middle
- if theyre close to the end points, it's easier to shift these points as the new endpoints




# Best Linear Predictor
using autocorrelation to get coefficients of past terms to predict next term
$\zeta_i = cov(Y, X_i)$ 
$\Delta_{ij}=Cov(X_i,X_j)$
coef vec = $\Delta^{-1}\zeta$

Is this like an AR model???


The PACF plot is defined as the hth coeficient of the BLP
- it is the correlation between $X_{t},X_{t-h}$ with all the terms in the middle removed