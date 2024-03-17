---
tags:
  - Math/statistic/correlation
---
# Correlation, $\rho$
### Description:
- Refers to any broad class of statistical relationships involving dependence
- The correlation of two random variables $X$ and $Y$, denoted by $\rho (X , Y )$
	- defined as long as $Var(X).Var(Y)$ is positive
	- Denotes the degree of linearity:
		- Near +1 or -1 denotes there is a high degree of linearity
		- Near 0 indicates such linearity is absent
### Correlation coefficient:
- $\displaystyle\rho(X,Y)={\color{tomato}\frac{\text{Cov}(X,Y)}{\sqrt{Var(X)Var(Y)}}}=\frac{n\sum x_iy_i-\sum x_i \sum y_i}{{\sqrt{n\sum x^2_i-(\sum x_i)^2}}.\sqrt{n\sum y^2_i-(\sum y_i)^2}}$  
	- $-1\le \rho(X,Y)\le 1$
	- $(x_i, y_i)$ are pairs of data for two variables $X$ and $Y$
- $\rho(X,Y)=1$ implies $m=\sigma_y/\sigma_x>0$ for $y=mx+c$
- $\rho(X,Y)=-1$ implies $m=-\sigma_y/\sigma_x<0$ for $y=mx+c$
### Degrees of correlation:
- Perfectly Correlated
	- Perfect positive vs perfect negative correlation
	- Has no margin of error
- [[Partly Correlation]]
- Uncorrelated
### [[Coefficient of Determination]]

### [[Spearman's Rank Correlation Coefficient]]