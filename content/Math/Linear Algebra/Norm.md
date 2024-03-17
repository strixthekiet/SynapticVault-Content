---
tags:
  - Math/linear/vector/norm
---
# Norm, $||\ . \ ||$
### Description:
- A norm on $\mathbb R^n$ is a real-valued **function** with special properties that maps any element $x\in \mathbb R^n$ i**nto a real number** (denoted by $||x||$)
- Must satisfy 3 conditions:
	- $\|x\|\geq0\ \forall x\in X, ||x|| = 0$ IFF $x = 0$
	- $\|x+y\|\leq\|x\|+\|y\|,$ for any $x, y \in X$  (triangle inequality)
	- $||\alpha x|| = |\alpha|.||x||$, for any $\alpha$ scalar and $x \in X$
### $l_p$ norm:
- $||\ . \ ||_p=\mathbb R^n \to \mathbb R$ 
- Defined as $\displaystyle |x|_{p}\doteq\left(\sum_{k=1}^{n}{\color{tomato}|x_{k}|^{p}}\right){\color{tomato}^{1/p}},\quad1\leq p<\infty$
### $p = 2$: 
- [[Euclidean Length]]
### $p = 1$: 
- sum-of-absolute-values length
- $|x|_{1}\doteq\sum_{k=1}^{n} |x_{k}|$
- $||x||_1=1$ forms a diamond
### $p = 0$: 
- -pseudo norm/the cardinality (number of non-zero elements)
- not a norm as it doesnt satisfy the last condition
### $p = ∞$: 
- max absolute value norm / [[Chebyshev Norm]]
- $|x|_\infty\doteq\operatorname*{max}_{k=1,\ldots,n}|x_{k}|$
- $||x||_{\infty}=1$ forms a square
---