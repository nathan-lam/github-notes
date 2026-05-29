

# Definition
A metric that measures how responsive a demographic is to a price change.
- This is calculated as the slop of a log-linear model

Total demand = Base demand * exp(elasticity * discount) if log-linear
- elasticity term is the metric


This builds on top of an existing demand model which assumes the typical demand without special pull factors


# Related
[[Uplift]] = average response to demand given price = price * elasticity
