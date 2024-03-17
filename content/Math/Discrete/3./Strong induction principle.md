---
mindmap-plugin: basic
tags:
  - Math/discrete/principle
---
# Strong induction
### Description:
- Allows us to make a stronger assumption in the inductive step. 
- Mathematical induction proves that we can climb as high as we like on a ladder, by proving that
	- we can climb on the bottom rung (base case) 
	- we can climb ==all== the previous rung then we can climb the next one
### Strong induction principle:
- At induction step $n + 1$, we have proved that all $P(k)$ for $k = 1, 2, . . . , n$ are true and thus we can use these facts to show $P(n + 1)$ is true as well:
	1. Base case:
		- First prove that $P(n)$ is true for some base values (e.g. $n=1,2$). These are base cases
	2. Inductive step:
		- Next prove that if $P(k)$ is true for $1\le k\le n$, then $P(n+1)$ is true. 
---