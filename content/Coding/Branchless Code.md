---
tags:
  - Coding
  - Tips
---

# Definition
An approach to coding that handles separate cases without using conditionals.

This is desired to avoid handling for every special case.
- Implies that all information flows back into a main stream
- It is impossible to maintain the different combination of conditionals

# Tricks

## Bools are Ints
An easy way to handle case A or case B is to store it in a boolean and utilize that in the calculation.
```python
x = "A"

use_A = x == "A"

y = 10 * use_A + 15 * (1-use_A) # outcome A * use_A bool + outcome B * not use_A

```

# Related
- [Branch Predictors](https://en.wikipedia.org/wiki/Branch_predictor)
	- when the compiler attempts to optimize and fails to predict 