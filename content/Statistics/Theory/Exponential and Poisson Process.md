---
tags:
  - Statistics/Theory
---
# Definition
A Poisson process can be defined by various ways

## Poisson Process Definition 1
- $N(0) = 0$ 
- $\{N(t),t\geq0\}$ independent increments
- $P(N(s+t)-N(s)=k)=\frac{(\lambda t)^ke^{-\lambda t}}{k!}$
	- each interval of length t is $Pois(\lambda t)$
## Poisson Process Definition 2
- $N(0) = 0$ 
	- No count given no time
- $\{N(t),t\geq0\}$ independent an stationary increments
	- each timeframe are the same and independent
- $P[N(t+h)-N(t)=1]=\lambda h+o(h)$
	- events are rare
- $P[N(t+h)-N(t)\geq2]=o(h)$
	- 2 or more events can't occur at the same moment
-  Therefore ${N(t),t\geq0} \sim Pois(\lambda),\lambda>0$ in timeframe t 

## Poisson Process Definition 3
- Let $T_{n} \overset{iid}{\sim} Exp(\lambda) \forall n\in\mathbb{N}$
- Let $S_n=\sum\limits^{n}_{i=1}T_i$ s.t. $S_0=0$
- Let $N(t), t\geq0$ be a counting process where the $n$th event happens at time $S_n$
	- $N(t) := max\{n: S_n\leq t\}$
	- $N(t)$ is the largest n that occurs within timeframe t
- Therefore ${N(t),t\geq0} \sim Pois(\lambda),\lambda>0$ in timeframe t



# Exponential Process
Often the **time** between events


Sum of Exp = Gamma
- Meaning the nth exponential event is $Gamma(n, \lambda)$

# Poisson Process
Often counting the number of events in a set time interval

Poisson is reasonable if:
- N(t) must be a counting number ($N(t) \in \mathbb{N}$)
- Less time gives less counts ($s\leq t \implies N(s)\leq N(t)$)
- Events between s and t = $N(t)-N(s)$ in $(s,t]$


This also applies between a starting and ending time
If the entire process is stationary (same process the entire duration), we can simplify
- $P(N(t)-N(s)=k) = P(N(t-s)=k)$

# Uniform
Ordering of events appears uniformly

This is the conditional distribution of the arrival times

Basically, events inside a time frame of a poisson process appear uniformly




# Summary

- Number of events in $[0,t], N(t) \sim Poisson(\lambda)$ 
- Time between events, $T_i\sim Exp(\lambda)$
- Sum of time between r events, $\sum^{r}_{i=1}T_i\sim \Gamma(r,\lambda)$
- Ordered events appear at a rate, $(T_{i}|N(t)=n)\sim Uniform(0,t)$
	- keep in mind the scope is different from interarrival times (no time frame) vs a fixed time frame






