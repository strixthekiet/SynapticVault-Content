---
tags:
  - Math/linear/vector
  - Math/statistic/correlation
---
# Vector's Correlation
### Description:
- Consider 2 [[De-meaned Vector]] $\tilde a,\tilde b$ from vector $a,b$
- The corresponding [[Correlation#Correlation coefficient|correlation coefficient]] is the **cosine** angle between the 2 de-meaned vectors:
	- $\displaystyle\rho(a,b):=\cos \angle(\tilde a, \tilde b)=\frac{\tilde a^T\tilde b}{||\tilde a||_2||\tilde b||_2} \in [-1,1]$ 
### Uncertainty of vector $x$:
- We can model uncertainty by the way of set $U$, we say $x\in U$, otherwise unknown.
- To model the lack of knowledge about a vector, we can use the uncertainty set, $U=\{ x\ : \ ||x-\hat x||\le  \rho\}$ 
	- where $\hat x$ is refered to the "nomial" model 
	- $\rho$ meansures the size of uncertainty around $\hat x$