---
tags:
  - Statistics/Plots
---
Receiver Operating Characteristic Curve
Measure the performance of a binary classifier

# Definition
A plot of the True Positive Rate vs False Positive Rate as thresholds vary
Specifically, it analyzes [[Sensitivity]] and [[Specificity]]


What is needed is are the actual outputs and predicted probabilities


| Y   | Y_hat prob |
| --- | ---------- |
| 1   | 0.6        |
| 0   | 0.3        |
| 0   | 0.7        |
| 1   | 0.8        |
| 1   | 0.45       |
As we vary a threshold \[0,1\], the predictions change whether they are correct or in correct.
For each threshold we plot (Sensitivty, 1- Sensitivity) based on varying the threshold for classifying
- $(\frac{\text{True Positive}}{\text{True Positive + False Negative}}, \frac{\text{False Positive}}{\text{False Positive + True Negative}})$
- $=(\frac{\text{True Positive}}{\text{All Actual Positives}}, \frac{\text{False positives}}{\text{All Actual Negatives}})$
- = (How often it is at predicting positive, How often it is predicting not postive)


The plot will form a concave plot, more area means the model prefers more True Positives than False Negatives




# Related
- [StatQuest](https://www.youtube.com/watch?v=4jRBRDbJemM)
