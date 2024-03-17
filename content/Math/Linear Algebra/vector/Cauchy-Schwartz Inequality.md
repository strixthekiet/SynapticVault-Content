---
tags:
  - Math/linear/vector
---
# Cauchy-Schwartz Inequality
### Description:
- ![[Drawing 2024-03-05 14.44.40.excalidraw]]
- From [[Euclidean Projection#Euclidean Projection on a line|Euclidean Projection on a line]], We have $|x^Ty|\le ||x||_2.||y||_2$ 
- The angle, $\theta$ defined by $\displaystyle \cos\theta=\frac{x^Ty}{||x||_2.||y||_2}$
- Implies that Cosine angle between 2 vector have magnitude less than one 
- $\to$ for any $n$-vector $y:\ \text{max}_{||x||_2\le 1} x^Ty=||y||_2$ 
### Generalized Cauchy-Schwartz Inequality:
- For any two vectors $\displaystyle x,y\in \mathbb R^n:\  |x^Ty|\color{tomato}\le  ||x||_p||y||_q$  where $\displaystyle \frac 1p +\frac 1q=1$
	- ex: $|x^Ty|\color{tomato}\le  ||x||_p||y||_q$
### Proof:
- WLOG, assume $||x||_2=1$ and show that $|x^Ty|\le ||y||_2$ for every $y$
- For every $t\in \mathbb R:$
	- $0\le ||tx-y||^2_2=t^2-2t(x^Ty)+||y||^2_2=(t-x^Ty)^2+||y||^2 - (x^Ty)^2$ 
- Pluggin $t=x^Ty$ proves the result