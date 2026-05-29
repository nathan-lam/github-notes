---
folder_desc:
tags:
  - Folder
  - Statistics/Inference/Hypothesis-Tests
---

# Definition
A comparison between two distributions (null vs alternative) to determine if both are the same or different.

It is often used as a procedure to determine if a measurement is significantly different from the null distribution.

Another way to put it is: "Is model A or B a better description of the data?"
- Model A and B are the null and alternative hypothesis



# What is it
A procedure for determining if a measurement is significant.
We make an assumption about the distribution of the measurement. Depending on how well the measurement matches the distributions, we reject or accept the null hypothesis

When we have a hypothesis, we have the mindset of wanting to reject it and this is enforced by saying "failed to reject the hypothesis"

# Terms
## [[P-value]]
The probability of obtaining the observed results (or more extreme) given the null hypothesis is true.
P-value = $P(X=x|H_0)=P(\text{Getting the observed data}|H_0=True)$

When the p-value is small, that's saying the null hypothesis created this really unlikely result. As a result, we reject the null hypothesis.


## Rejection Region
The portion on the distribution that determines if we reject the null hypothesis if the p-value lands here. 

## Type 1 Error
False Positive - The experiment detects something present when there's nothing
We address false positives by tuning the significance level ($\alpha$) 

## Type 2 Error
False Negative - The experiment does not detect anything present when there's something
We address false negatives by tuning the power (1-$\beta$)



# Variations



## One-Tailed Test
Stronger than a 2-tail if the hypothesis is correct

A Left Tailed Test 

## Two-Tailed Test
Considers 
The critical value (cut off points) are equally spread out on both ends of the distribution.
- The area of both rejection regions should add to the significance level

The rejection region will be like the tail bits on both ends of a normal distribution



## Parametric vs Nonparametric tests
Parametric tests assume a distributions while nonparametric tests do not
A parametric test will tend to be more powerful than a nonparametric test

# List of tests
```base
views:
  - type: table
    name: Table
    filters:
      and:
        - file.inFolder("04 Notes/Disciplines/Statistics/Hypothesis Tests")
        - '!file.tags.contains("Folder")'
    order:
      - file.name
      - hypothesis_distribution
      - hypothesis_parameter
      - hypothesis_null
      - hypothesis_alt
    sort:
      - property: hypothesis_distribution
        direction: ASC
      - property: title
        direction: ASC

```

