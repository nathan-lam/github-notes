---
hypothesis_distribution: None
hypothesis_parameter: None
tags:
  - Statistics/Hypothesis-Test
---
# Application
Could the results of data between 2 groups happen by random shuffling


# Hypothesis
$$H_{0}: \mu_1-\mu_2 = 0$$
$$H_{A} : \mu_1-\mu_{2}\neq0$$
# General Assumptions
- Results were achieved regardless of the group
	- Assumes every sample is "destined" to give the results they gave
	- 

# Algorithm
```R
# experiment details
sampleSize <- 100 # split into 50-50 groups
treatmentSuccess <- 43
controlSuccess <- 37
treatment <- c(rep(TRUE, treatmentSuccess),
			   rep(FALSE, 50-treatmentSuccess))
control <- c(rep(TRUE,controlSuccess),
			 rep(FALSE, 50-controlSuccess)
experiment <- c(treatment, control)
obs_diff <- mean(treatment) - mean(control)

# running the randomization test
nTrials <- 10000
differences <- rep(NA, nTrials)
for(i in 1:nTrials){
	random_mixing <- sample(experiment)
	treatment <- random_mixing[1:50]
	control <- random_mixing[51:100]
	differences[i] <- mean(treatment) - mean(control)
}
mean(abs(differences) >= obs_diff) # 2 tail test
mean(differences >= obs_diff) # 1 tail test

```

```
put number of successes and fails into list of treatments
put number of successes and fails into list of control
record observed difference

diff_list = list to preallocate random sample differences

looping a bunch of times
	sampled_experiment = experiment sampled without replacement
	sampled_treatment = sampled_experiement indicies for treatment 
	sampled_control = sampled_experiment indices for control
	diff_list[i] = mean(control) - mean(treatment)

p_val = mean(abs(diff_list) > observed difference) # 2 tail test
```

