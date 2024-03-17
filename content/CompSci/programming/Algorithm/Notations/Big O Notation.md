---
tags:
  - CompSci/programming/Algorithm
aliases:
  - Order of Growth
---
# Big O Notation
### Description:
- $f(n)$ is $O(g(n))$ if there exist constants $c>0$ and $n_0\ge 0$ such that $0\le f(n)\ {\color{tomato}\le}\ c.g(n)$ for all $n\ge n_0$ 
	- where $f(n)$ denotes the worst-case running time
	- ie. only $2n^2\to n^2$
### Common mistake:
- $g_1(n)=10 n^3$ and $g_2(n)=n^3$
- $g_1(n)=g_2(n)= O(n^3)$  but $g_1(n)\not = g_2(n)$ 
### Properties:
- Reflexivity: $f$ is $O(f)$
- Constants: if $f$ is $O(g)$ and $c>0$, then $cf$ is $O(g)$
- Products: if $f_1$ is $O(g_1)$ and $f_2$ is $O(g_2)$ then $f_1+f_2$ is $O(\text{max}\{g_1,g_2\})$
- Transitivity: if $f$ is $O(g)$ and $g$ is $O(h)$ then f is $O(h)$
### With multiple variables:
- $f(m,n)$ is $O(g(m,n))$ if there exist constants $c>0$ and $m_0,n_0\ge 0$ 
- such that $0\le f(m,n)\le c.g(m,n)$ for all $n\ge n_0,m\ge m_0$
	- ex: $f(m,n)=32mn^2+17n^3$ is both $O(mn^2+n^3)$ and $O(mn^3)$
	- $f(n)$ is $O(n^3)$ if there is condition that implies $n>m$
	- $f(m,n)$ is neither $O(n^3)$ nor $O(mn^2)$
