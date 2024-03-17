---
tags:
  - CompSci/programming/Algorithm
---
# Big Omega Notation
### Description:
- $f(n)$ is $\Omega(g(n))$ if there exist constants $c>0$ and $n_0\ge 0$ such that $f(n){\color{tomato}\ge } c.g(n)$ for all $n\ge n_0$ 
	- where $f(n)$ denotes the worst-case running time
	- ie.$f(n)=32n^2+17n+1\to f(n)$ is both $\Omega(n^2)$ and $\Omega(n)$
	- lower bound
