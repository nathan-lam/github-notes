---
hypothesis_distribution: Chi-Squared
hypothesis_parameter: df
tags:
  - Statistics/Hypothesis-Test
---
# Application
Categorical analysis


# Hypothesis


# General Assumptions
- 80% of the entries must have **Expectation** at least 5 counts
	- This is a conservative assumption
- Valid for small sample size where Chi Square fails
- 

# Variations


## Goodness of Fit
Tests if something follows a multinomial distribution
- 1 Categorical input
- 1 Continuous output

|            | Col 1 | Col 2 | Col 3 |
| ---------- | ----- | ----- | ----- |
| Variable A |       |       |       |
Does A follow this hypothesized distribution?
df = num col - 1

## Test of Independence
Tests if two variables are independent
- 2 categorical input
- 1 Continuous ouput


|     | A.1 | A.2 | A.3 |
| --- | --- | --- | --- |
| B.1 |     |     |     |
| B.2 |     |     |     |
| B.3 |     |     |     |
Are A and B independent?
df = (num col– 1)\*(num rows – 1)

## Test of Homogeneity
Tests if 2 distributions are the same
- comparing 2 multinomial distributions


|            | Col 1 | Col 2 | Col 3 |
| ---------- | ----- | ----- | ----- |
| Variable A |       |       |       |
| Variable B |       |       |       |
Are A and B the same?
df = num col - 1


# Application

## R
chisq.test()
Can use a monte carlo simulatation to get the p-values, this [conditions on marginals](https://stats.stackexchange.com/questions/81483/warning-in-r-chi-squared-approximation-may-be-incorrect)
Applying the simulation means it [overcomes the issue with low data count](https://stats.stackexchange.com/questions/57228/quantifying-the-overlap-in-sort-task-results-with-cells-5)
	also from [this](https://stats.stackexchange.com/questions/62445/rules-to-apply-monte-carlo-simulation-of-p-values-for-chi-squared-test)


# Related
https://openstax.org/books/statistics/pages/11-introduction
- [[Goodness of Fit Test]]
- [[Test of Independence]]
- [[Test of Homogeneity]]
