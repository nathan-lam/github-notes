---
tags: Mathematics, Statistics
---

# Definition
A way to minimize false negatives



Type 1 Error = $P(reject H_{0}|H_{0}= True) = \alpha$ = False positive

Type 2 Error = $P(accept H_{0}|H_{0}= False)=\beta$ = False negative

$Power=1-\beta$


The p-value minimizes false positives ($\alpha$)



$H_{0}:\mu_x-\mu_y=c$
$H_{1}:\mu_x-\mu_y=\Delta$
$\Delta$ is the true difference

Power = probability test statistic falls in the rejection region
$Power = P(|\bar{X}-\bar{Y}| > dist*sd|H_{1}= True) = P(\bar{X}-\bar{Y} > dist*sd) + P(\bar{X}-\bar{Y} < -dist*sd)$
These are the tails

$Power = 1-cdf(dist*sd) + cdf(-dist*sd)$ 


### Steps
1. Get the test statistic
2. Find critical boundary that will determine accept or reject
3. Find the corresponding boundaries in the alternative hypothesis
4. The area in the rejection region, marked by the boundaries = Power
5. Turn power into a function of n

### Example
2 sample z test
$D = \bar{X}-\bar{Y}$
$H_{0}: D = 0$
$H_{a}:D\ne 0$ or equivalently: $H_{a}:D=\Delta$

$Var(D) = Var(\bar{X}-\bar{Y}) = \sigma^{2}(\frac{1}{n}+\frac{1}{n})= \frac{2\sigma^2}{n}$

so we have 
	$H_{0} \implies D \sim Normal(0,\frac{2\sigma^2}{n})$
	$H_{A}\implies D\sim Normal(\Delta,\frac{2\sigma^2}{n})$



$Power = P\left(|D| > z\left(\frac{\alpha}{2}\right)sd(D)\right)$
$Power$ = $P\left(D < -z(\frac{\alpha}{2})\sigma\sqrt{\frac{2}{n}}\right)$ + $P\left(D > z(\frac{\alpha}{2})\sigma\sqrt{\frac{2}{n}}\right)$ = left tail + right tail
$Power$ = $P\left(\frac{D=\Delta}{\sigma\sqrt{\frac{2}{n}}}<-\frac{z(\frac{\alpha}{2})\sigma\sqrt{\frac{2}{n}}-\Delta}{\sigma\sqrt{\frac{2}{n}}}\right )$  + $P\left(\frac{D=\Delta}{\sigma\sqrt{\frac{2}{n}}}>\frac{z(\frac{\alpha}{2})\sigma\sqrt{\frac{2}{n}}-\Delta}{\sigma\sqrt{\frac{2}{n}}}\right )$ , shift to standard normal
$Power$ = $P\left(\frac{D=\Delta}{\sigma\sqrt{\frac{2}{n}}}<-z(\frac{\alpha}{2})-\frac{\Delta}{\sigma}\sqrt{\frac{2}{n}}\right )$  + $P\left(\frac{D=\Delta}{\sigma\sqrt{\frac{2}{n}}}>z(\frac{\alpha}{2})-\frac{\Delta}{\sigma}\sqrt{\frac{2}{n}}\right )$
 = $P\left(\frac{D=\Delta}{\sigma\sqrt{\frac{2}{n}}}<-z(\frac{\alpha}{2})-\frac{\Delta}{\sigma}\sqrt{\frac{2}{n}}\right )$  + $1-P\left(\frac{D=\Delta}{\sigma\sqrt{\frac{2}{n}}}<z(\frac{\alpha}{2})-\frac{\Delta}{\sigma}\sqrt{\frac{2}{n}}\right )$
$=\Phi\left(-z\left(\frac{\alpha}{2}\right)-\frac{\Delta}{\sigma}\sqrt{\frac{2}{n}}\right)$ + 1$- \Phi(z(\frac{\alpha}{2})-\frac{\Delta}{\sigma}\sqrt{\frac{2}{n}})$


plug in various power, $\Delta$, n levels to determine desired effects

### Rule of Thumb
Assuming a 2 sample t test with power = 80%, sig level = 5%
$n=16\frac{s^2}{d^2}$
s = population variance estimate
d = difference