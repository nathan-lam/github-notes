---
tags:
  - Statistics/Models
---

A model that captures both signal and noise

An alternative to regression + ARMA

# Model
Seasonal
Auto Regressive
Integrated (differencing)
Moving Average

This combines all of them
- Differencing captures trend
	- Differencing offset captures seasonality
- AR + MA can model noise

The seasonality shifts the differencing to an offset: $X_{10}-X_{9} \rightarrow X_{10}-X_{5}$


# Components
A stationary solution is unique if the roots != 1

## AR
- An AR fit is unique iff the fit is invertible (|coef| > 1)


## MA
- A MA fit is unique iff the fit is causal (|coef| > 1)

## Differencing



# Diagnosis

[[ACF Plot]] to identify MA model
[[PACF Plot]] to identify AR model

## Ljung Box Pierce test
A Chi Squared test if an ARMA(p,q) works

This uses the Box Pierce test statistic, which is a sum of errors^2
The Ljung Box Pierce modifies this a bit

# Resources



# Related