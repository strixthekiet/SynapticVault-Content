---
tags:
  - CompSci/programming/Algorithm
---
# Big Theta Notation
### Description:
- $f(n)$ is $\Theta(g(n))$ if there exist constants $c_1,c_2>0$ and $n_0\ge 0$ such that $0\le {\color{tomato}c_1}g(n) \le f(n) \le {\color{tomato}c_2}g(n)$ for all
	- where $f(n)$ denotes the running time
	- ie.$f(n)=32n^2+17n+1\to f(n)$ is $\Theta(n^2)$ for $c_1=32,c_2=50,n_0=1$
		- not $\Theta(n)$ nor $\Theta(n^2)$
	- 
