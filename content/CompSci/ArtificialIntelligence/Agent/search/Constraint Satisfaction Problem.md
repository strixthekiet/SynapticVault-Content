---
tags:
  - CompSci/AI/Agent/Search
aliases:
  - CSP
---
# Constraint Satisfaction Problem
### Description:
- Assumptions about the world: 
	- a single agent
	- deterministic actions
	- fully observed state
	- discrete state space
- Plan a sequence of actions
- Same as [[Search Problem]] but neighbors of a state might be constrained due to the path so far
- Identification: assignments to variables
	- The goal it self is important
	- All paths at the same depth (for some formula)
	- Specialized class of identification problems
- Goal test is a set of constraints specifying **allowable combinations of values for subset of variable**
- $O(d^n)$
### Variable:
- State is defined by variable $X_i$ with values from a domain $D_i$
- Discrete vs continous vairbles:
	- Discrete:
		- Finite domains:
			- Size $d$ means $O(d^n)$ complete assignments
		- Infinite domains (integers, strings,..)
			- Linear constaints are solvable, non-linear are not
			- ex: job scheduling, variables can be start/end of the job
	- Continuous
		- Linear constants are solvable in polynomial time in LP methods
### Constraints:
- Unary constraint:
	- involve a single variable
	- ex: in map coloring, NY != green
- Binary constraints:
	- involves a pair of variables
	- ex: Hanoi != Halong
- Higher-order constraints:
	- invole 3 or more variables
	- ex: sudoku,
- Preferences (soft constraints)?
	- Sometimes the 1 assignment is prefered over the other
	- Can be represented by cost of the variable assignment
### A few example:
- [[Graph Coloring|Map Coloring]]
- [[N-Queens Problem]] , what is the maximum number of queens can stand on a board that none of them is on attack range of another
- Sudoku:
	- each non-default square is a variable
	- Domains are from 1 to 9
### [[Constraint Graph]]