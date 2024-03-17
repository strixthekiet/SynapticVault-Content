---
tags:
  - Math/statistic
---
# Population Proportion
### Description:
- True population proportion $p$ is unknown
- $\displaystyle \bar p= \frac X n$ 
	- where $X$ is [[Binomial distribution|binomial random variable]] denotes the number of successes in the sample
	- $X\sim B(n,p). E[X]=np$ and $\sigma_X=\sqrt{npq}$
- $E[\bar p]=p$ and $\sigma(\bar p)=\sqrt{\frac{pq}{n}}$
### Inteference about $p_1-p_2$:
- The difference between 2 population proportions is $p_1-p_2$
- Let $\bar p_1, \bar p_2$ be the saple proportion for a random sample from population 1 and 2
- $E[\bar p_1-\bar p_2]=p_1-p_2$ and $\displaystyle \sigma_{\bar p_1-\bar p_2}=\sqrt{\frac{p_1(1-p_1)}{n_1}+\frac{p_2(1-p_2)}{n_2}}$ 
- If $n_1\bar p_1\ge 5$ and $n_1\bar q_1\ge 5$ and $n_2\bar p_2\ge 5$ and $n_2\bar q_2\ge 5$
	- The sampling distribution of $\bar p_1-\bar p_2$ can be approximated by normal distribution
	- $\displaystyle CI(\alpha \%)=\bar p_1-\bar p_2\pm z_{\alpha/2}\sqrt{\frac{p_1(1-p_1)}{n_1}+\frac{p_2(1-p_2)}{n_2}}$ 
