---
mindmap-plugin: basic
tags:
  - Math/discrete
aliases:
  - induction
---
# Induction
### Description:
- Mathematical induction proves that we can climb as high as we like on a ladder, by proving that: 
	- we can climb onto the bottom rung (the basis) 
	- and that from each rung we can climb up to the next one (the step)
### The induction principle (ordinary induction):
- Let $P$ be a predicate on a non-negative integers. If
	- Inductive hypothesis:
		- $P(0)$ is true
	- Inductive step:
		- $P(n)$ ==implies== $P(n+1)$ for all non-negative integers $n$, 
	- then: $P(m)$ is true for all non-negative integers, $m$
### [[Strong induction principle]]
