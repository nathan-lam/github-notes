---
tags:
  - Statistics/Models
---


# Definition

Splitting the dataset into random train/test set to estimate predictive ability


# Variations
Do keep in mind that each data point should be **interchangeable**. Data that relies on sequential data (like time series) can be done but need to be prepared carefully

## Leave One Out Cross Validation
Creates n train/test splits where each datapoint is left out

This creates highly correlated training sets which can lead to overfitting


## K-fold Cross Validation
Creates k groups which each take turns being the test set

This creates less correlated training sets


## Incremental Cross Validation
Used for time series where sequential data holds structure


1. Define a model
2. Split train and test
3. For each new observed data point from test
	1. Fit the model
	2. evaluate the errors^2
4. Average error squares across each step is the evaluation for this model

This incrementally measures the predictive error as more sequential data is observed
Pick the model with the least MSE

# Limitations
The goal of cross validation is to create more datasets of novel scenarios for the model to train on.
If each (sub)dataset are too correlated then cross validation fails to generalize.

A way to alleviate this is to allocation another chuck of data for the best cross validated model to evaluate on.


# Resources


# Related
- [[Ensemble Methods]]
- [[Bootstrapping]]
