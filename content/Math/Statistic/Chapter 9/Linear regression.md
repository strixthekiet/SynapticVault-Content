---
tags:
  - Math/statistic
  - CompSci/AI/ML/model/linear
aliases:
  - Linear prediction
  - Line of best fit
---
# Linear regression
### Description:
- [[Prediction]] by [[Regression Model]]
- Actual value of $y=\beta_0 +\beta_1 +\epsilon$
	- Regression equation$\implies E(y)=\beta_0+\beta_1 x$
- Predicted valye of $\displaystyle \hat y=b_0 +b_1 x$
	- $\hat y$ is the point estimator of $E(y)$
- In practice, $\beta_0$ and $\beta_1$ are not known, but can be estimated with $b_0$ and $b_1$
	- where $b_0$ and $b_1$ are computed by least squares method
- Some notations:
	- $x^*$: given value of independent value of $x$
	- $y^*$: possible values (a range) of dependent value of $y$ when $x=x*$
	- $\hat y^*=b_0 +b_1x^*$: the point estimator $E(y^*)$ and the predictor of an individual value of $y^*$ when $x=x^*$
### Finding line of best fit:
- There are 2 main methods:
	1. Scattergraph method:
		- Draw a line through data points with about an equal number of points above and below the line. 
	2. Linear regression:
		- Using correlation:
			- We need to choose $a$ and $b$ to minimize the [[Mean square error]]
			- ${\color{tomato}E [(Y − (a + bX ))^2]} =E [Y^2] − 2aE [Y ] − 2bE [XY ] + a^2 +2abE [X ] + b^2E [X ^2]$
			- Taking partial derivative and set them equal to 0 we have $a$ and $b$ when it is at minimum point
				- Cant have maximum due to the nature of the problem
			- $\displaystyle b=\frac{\text{Cov}(X,Y)}{\sigma^2_X}$
			- $a=E[Y]-bE[X]$
			- The best linear predictor (lowest mean square error) is: $\mu_y+\frac{\rho\sigma_y}{\sigma_x}(X-\mu_x)$
				- Happens when $\mu_y=E[Y],\mu_y=E[X]$ and $\rho$ is the [[Correlation]] of $X$ and $Y$
				- The [[Mean square error]] of this predictor is given by $\displaystyle E[(Y -\mu_y - \frac{\rho\sigma_y}{\sigma_x}(X - \mu_x )^2]= \sigma^2_y (1 - \rho^2)$
		- Using $y=a+bX$:
			- $\displaystyle b=\frac{n\sum x_iy_i-\sum x_i \sum y_i}{{\sqrt{n\sum x^2_i-(\sum x_i)^2}}}$ 
			- $\displaystyle a=\frac{\sum y}n -\frac{b\sum x}{n}$
### Assumptions about $\epsilon$ in linear regression model:
1. $E (\epsilon) = 0$. This implies $\beta_0$ and $\beta_1$ are constants, and hence $\color{tomato} E (y ) = \beta_0 + \beta_1 x$ 
2. The variance of $ε$, denoted by $σ^2$, is the same for all $x$
3. The values of $ε$ are independent.  
4. $ε$ is a normally distributed random variable for all values of $x$ 
### [[Regression Model#Testing for significance|Testing for significance]] of linear:
- If $β_1 = 0$, then $E(y ) = β_0$. In this case, we would conclude that $x$ and $y$ are not linearly related
- If $β1 \not = 0$, we would conclude that the two variables are related. 
- The [[t test]] is commonly used. 
	- It requires an estimate of $σ2$, the variance of $ε$ in the regression model.  
- With $\hat y = b_0 + b_1x$, we can use the [[Mean square error]] $s^2$ as an estimate $σ^2$
	- $\color{tomato}\displaystyle s^2 =  \frac{\sum(y_i − \hat y_i )^2}{ n − 2}$
	- The standard error of the estimate $s = \sqrt{s^2}$ is used to estimate $σ$
- $H_0: \beta _1 =0, H_a:\beta _1\not =1$
- For sample distributin of $b_1$:
	- Expected value: $E(b_1)=\beta_1$
	- sd: $\displaystyle \sigma_{b_1}=\frac{\sigma}{\sqrt{\sum(x_i-\bar x)^2}}$
		- then we use it to estimate: $\displaystyle s_{b_1}=\frac{s}{\sqrt{\sum(x_i-\bar x)^2}}$ 
	- $b_1\sim N(\beta_1,\sigma^2_{b_1})$ 
	- $\displaystyle \to ts=\frac{b_1-\beta_1}{s_{b_1}}=\color{tomato}\frac{b_1}{s_{b_1}}$ 
	- Reject $H_0$ if $p$-value $\le \alpha$, where $p$ follows a [[t distribution]] with $n-2$ degrees of freedom
- Confidence Interval for $\beta_1$ is $\color{tomato} b_1\pm t_{\alpha/2}s_{b_1}$
	- with two-tailed
	- If the CI include 0, we can hypothesize value of $\beta_1$ might not be in the CI
	- We can reject $H_0$ as there is a chance the model is not significant enought to be used
### Variance of predicting value:
- $\displaystyle Var(\hat y^*)=s^2_{\hat y^*}=s^2.\bigg[\frac 1n + \frac{(x^*-\bar x)^2}{\sum{(x_i-\bar x)^2}} \bigg]$ 
	- where $s^2$ is the variance of the all collected $y$
### Confidence interval for mean of predicting value $E(y^*)$:
- [[Confidence interval]] of the mean of all predicting value when $x=x^*$
- $\displaystyle CI((1-\alpha)\%)=\hat y^*\pm t_{\alpha/2} s_{\hat y^*}$
	- with $n-2$ degree of freedom
### [[Prediction]] interval for $\hat y^*$:
- [[Confidence interval]] of the 1 value when $x=x^*$, thus more uncertainty
- Has variance of [[Mean square error]] and [[#Variance of predicting value]]:
	- $\displaystyle s^2_{pred}=s^2+s^2_{\hat y^*}=s^2.\bigg[ 1+\frac 1n +\frac{(x^*-\bar x)^2}{\sum{(x_i-\bar x)^2}}\bigg]$ 