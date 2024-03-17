---
mindmap-plugin: basic
tags:
  - Math/discrete/definition
aliases:
  - Fermat's method of descent
---
# Infinite descent principle
### Description
-  There is no infinite sequence of strictly decreasing non-negative integers #Math/discrete/theorem 
- Used to show that a statement cannot possibly hold for any number
	- by showing that if the statement were to hold for a number
	- then the same would be true for a smaller number
	- leading to an infinite descent and ultimately a contradiction.
- The method relies on [[Well ordering principle]], so only a finite number of non-negative integers are smaller than any given one
- A method of [[Proof by contradiction]]
- Used to solve [[Fermat's last theorem#For $n=3$|Fermat's last theorem for n=3]] and [[Fermat's last theorem#For $n=4$|4]]
### Proof by infinite descent principle
- Originally (to prove all $P_n$ is false)
	- Let $m$ be a positive integer. 
	- Suppose that whenever $P(m)$ holds for some $m>k$, there exists a positive integer $j$ such that $m>j>k$ and $P(j)$ holds. 
		- $m$ must be the smallest by [[Well ordering principle]]
	- Then $P(n)$ is false for all positive integers $n$.
- Equivalently  (to prove all $P_n$ is true)
	- Let $P$ be a predicate on nonnegative integers. Assume that 
		- $P(0)$ is a true statement (the smallest ) and  
		- for all $k ∈ N$, if the statement $P(k)$ is false then there exists a natural number $m, m < k$, for which the statement $P(m)$ is also false. 
			- By induction, it would make $P(0)$ also false, therefore, $P(K)$ has to be true
	- Then, the statement $P(n)$ is true for all natural numbers $n ∈ N$
