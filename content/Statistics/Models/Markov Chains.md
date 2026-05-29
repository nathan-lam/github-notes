---
tags:
  - Statistics/Theory
---

# Definition
A stochastic process where a sequence of random events depend on the previous state.

A stochastic process is a Markov Chain if a sequence of random variables only relies on the previous term.
$$
P(X_{t+1}|X_t,X_{t-1},\dots,X_0) = P(X_{t+1}=s|X_t) \forall t\geq0, \forall s 
$$

This relation can be expressed as a transition matrix from one state to another


# Properties

## Accessible and Communicative
State j is accessible if state i has a probability of reaching j

Communicative is the 2 way version of the, i can reach j and vice versa in finite time

### Communication Properties
- Reflexive: i -> i
- Symmetric: i-> j and j -> i (also means i, j are in the same class)
- Transitive: i -> j -> k = i -> k

## Transient and Recurrent
If a state will eventually return, it is recurrent.
If it will never return, it is transient

## Irreducible
If a graph cannot be pruned without changing the state relations
If a class cannot be remove without changing the graph

## Absorbing
Never escape once entered

## Periodicity
If a state returns to itself in finite time

Positive recurrent = eventually come back in finite time
null recurrent = never come back in infinite time

### Periodicity Properties
- if i and j are symmetric, then they have the same period time
