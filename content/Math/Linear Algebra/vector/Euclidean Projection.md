---
tags:
  - Math/linear/vector
---
# Euclidean Projection
### Description:
- Corresponds to the problem of finding a point on a given set that is closest (in Euclidean length) to a given point
- Given a vector $x$ in $\mathbb{R}^n$ in a closed set $S\subseteq \mathbb R^n$, the project of $x$ onto $S$, denoted as $\sqcap_S(x)$, is defined as the point in $S$ at minimal distance from $x$
	- S can be a line, a plane, hyperplane
- $\sqcap_S(x)=\text{arg }\text{min }_{y\in S} ||y-x||_2$ 
	- arg refers to the unique minimizer
### Euclidean Projection on a line:
- Denotes $L=x_0+span(u)$
	- $u$ is the direction of the line. WLOG, let $||u||_2=1$
- Let $p\in \mathbb R^n$ be a given point 
	- $p^*$ be the point on the line that is project of $p$
- $p^*=\text{arg }\text{min }_{x\in S} ||x-p||_2$ 
	- $p^*$ such that it minimizes $x-p$
- As any point on $L$ can be written as $x=x_0+t.u$ for a scalar $t$, then we need to minize the $t^*$ (value of $t$ for $p^*$) $\to$ minimize $f(t):= ||tu-(p-x_0)||^2_2$
- A lot more proofs, then we have,$t^*=u^T(p-x_0)$ and $|u^Tp|\le ||p||_2$ 
###
---