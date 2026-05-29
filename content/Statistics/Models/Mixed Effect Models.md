---
tags:
  - Statistics/Models
---
Modeling with Interaction effects with no baseline comparison, only a general baseline comparison

# Definition
Typical modeling assumes a homogenous sample

Mixed Effects means we consider hierarchical groups within the sample (not homogenous)
- there might be difference between subgroups

Similar to interaction effects but not the same, but interactions can also be included

Mixed Effects considers Fixed and Random Effects
- There is no hard rule to determine what is what
- fixed = attributes that are shared between groups
- random = the variation between groups



# Example
Treatment used for body weight
- Each people are their own group
	- People vary in weight (we dont care about this variation between groups)
fixed = weeks in treatment
random = body weight

If we assume a Random Intercept (random starting body weight but fixed weight loss)
- we fit a model to each group, no single category as a baseline
	- an overall effect is measure and variation is in reference to that
- this differs from base [[Linear Regression]] which needs a baseline category



# Related
- [[Linear Regression]] but a different view on [[Interaction effects]]
- Repeated Measures [[ANOVA Test]]
	- similar to how categorical variables may affect a continuous variable
	- cannot handle missing values unlike Mixed Effect Models
- videos
	- https://www.youtube.com/watch?v=QCqF-2E86r0
	- https://www.youtube.com/watch?v=4bGG02Jsjyc
- https://glennwilliams.me/r4psych/mixed-effects-models.html

