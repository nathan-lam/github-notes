---
tags:
  - Statistics/Plots
knowledge_classes:
  - UCB-stat153
aliases:
  - Autocorrelation Function Plot
---
AutoCorrelation Function Plot

# Definition
A plot of a dataset's correlation with itself per lag step
- Correlation with itself shifted by some lag k

This effect can be from both direct and indirect dependence

# Usage
The bands indicate a 95% confidence interval

The number of lags above the band indicate the argument of a MA model

- White Noise
	- all lags inside the band indicates white noise
	- non-randomness will result in significant lags
- Stationarity
	- Fast decline if stationary; else non stationary
- Trends
	- trends will have a slow decline; close points have similar values
- Seasonality
	- will appear as wavy; resonating frequencies will appear higher + the decline

# Libraries
- R: acf
- from statsmodels.graphics.tsaplots import plot_acf

# Related


# Sources
https://en.wikipedia.org/wiki/Autocorrelation
https://statisticsbyjim.com/time-series/autocorrelation-partial-autocorrelation/