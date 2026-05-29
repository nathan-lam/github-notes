---
tags:
  - Algorithms
---
# Definition
A methods of getting better predictions by aggregating many submodels together

# Bagging
Batch Aggregating

1. Starting with a sample and number of interested submodels
2. For each submodel, fit using a bootstrapped sample
3. Get a prediction by feeding the inputs into the model then averaging the outputs


Pros

Cons
- Submodels are highly correlated due to similar bootstrapped samples

# Random Forest

1. Start with a sample and number of interested submodels
2. For each submodel, randomly sample features then fit using a bootstrapped sample
3. Get a prediction by feeding the inputs into the model then averaging the output

Pros
- Removes issue of correlated models found in Bagging
Cons
- Computationally intensive

# Boosting