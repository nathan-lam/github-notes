---
tags:
  - Statistics/Plots
---
Partial AutoCorrelation Function Plot

# Definition
A plot of a dataset's correlation with itself AFTER removing the effects of shorter lags
It controls for other lags
ex. PACF(3) = correlation not explained by lags 1, 2


# Usage
The bands indicate a 95% confidence interval

The number of lags above the band indicate the argument of a AR model

# Libraries
- pacf (base R)
- from statsmodels.graphics.tsaplots import plot_acf (python)

# Related



# Sources
https://en.wikipedia.org/wiki/Partial_autocorrelation_function
https://statisticsbyjim.com/time-series/autocorrelation-partial-autocorrelation/

