---
hypothesis_distribution: Multinomial
tags:
  - Statistics/Hypothesis-Test
---
The distribution of leading digits

It's the natural distribution of measures under a process that grows
- have to go through starting with 1's before starting with 2's
# Applications
Elections
Finance
Anything with measured numbers that range several magnitudes


# Hypothesis
Benford's law is a multinomial distribution, so [[Chi Squared Test#Goodness of Fit]] can be used to verify
$$
\begin{aligned}
H_{0}&: \text{prop of nth digit} = log(1+\frac{1}{n})\forall n\in\{1,2,...,9\}\\
H_{a}&: \exists n \text{ s.t. }\text{prop of nth digit} \neq log(1+1/n)
\end{aligned}
$$
ALL digits roughly follow the distribution

Rejecting the null is a flag to investigate, natural data might naturally break benfords law
- not proof of fraud

df = number of groups - 1 = 9 - 1 = 8

Hypothesis test is very strict, close enough shape is fine
fraud + still looks like benfords > fraud + not looks like benfords
- still second and last digit test

# Assumptions
- Data must be measured (numerical)
	- not categorical numbers (ID, phone numbers, zip codes)
	- they should not be assigned even as a number, like hourly wage
- Data must span several orders of magnitudes; more = better
	- implies data must be unbounded
- More data is better

It's also good to check the literature
- [Law of Anomalous Numbers - The original paper by Benford](https://www.jstor.org/stable/984802)
- [Benford's Law and the Detection of Election Fraud](https://www.cambridge.org/core/journals/political-analysis/article/benfords-law-and-the-detection-of-election-fraud/3B1D64E822371C461AF3C61CE91AAF6D)
- [Comment on “Benford's Law and the Detection of Election Fraud”](https://www.cambridge.org/core/journals/political-analysis/article/comment-on-benfords-law-and-the-detection-of-election-fraud/BC29680D8B5469A54C7C9D865029FE7C)


# Related
- [Why do Biden's votes not follow Benford's Law?](https://www.youtube.com/watch?v=etx0k1nLn78)
	- The second digit test
		- just use the formula to add all the second digits ending in d
	- The last digits test ~ uniform (assuming a large magnitude)
		- signals if rounding has been used
- [Statology](https://www.statology.org/benfords-law/)
- [Statisticsbyjim](https://statisticsbyjim.com/probability/benfords-law/)