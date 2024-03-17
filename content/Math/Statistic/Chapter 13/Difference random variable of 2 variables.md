---
tags:
  - Math/statistic/test
---
# Difference random variable of 2 variables
### Description:
- The variable is made from minusing one datapoint to the otehr
### When $\sigma$ is known:
- When $n$ tends to larger, $\displaystyle \bar x_1 -\bar x_2\sim N\bigg( {\color{tomato}D_0}, {\color{tomato}\sqrt{\frac{\sigma^2_1}{n_1}+\frac{\sigma^2_2}{n_2}}}\bigg)$
	- $D_0=\mu_1-\mu_2$
### When $\sigma$ is unknown:
- When $n$ tends to larger, $\displaystyle \bar x_1 -\bar x_2\sim T\bigg( {\color{tomato}D_0}, {\color{tomato}\sqrt{\frac{s^2_1}{n_1}+\frac{s^2_2}{n_2}}}\bigg)$
	- with df
### Match samples:
- To see when the 2 samples have the same mean by collecting $n$ samples from each 
- Let $\displaystyle d=x_a-x_b$
	- $\displaystyle \to \bar d =\frac{\sum d_i}{n}, s_d=\sqrt{\frac{\sum(d_i-\bar d)^2}{n-1}}$ 
	- $\to H_0: \mu_d=0, H_1: \mu_d\not= 0$
---
