---
mindmap-plugin: basic
tags:
  - Math/discrete/definition
aliases:
  - relation
---
# Relation

### Definition:
- A binary relation, R, consists of a [[Set|set]] A, called domain of R, a set B, called codomain of R, and a [[Set#Subset $A subset B$ math/discrete/definition|subset]] of graph of $R$​
	- We write $R: A\to B$ to indicate that R is a relation from A to B
	- “$a R b$: the pair $(a,b)$ is in the graph of R, means $a$ and $b$ belongs to $R$
	- For every [[Ordered tuples|ordered tuple]] pair, $(x,y)\in R, x\in A, y\in B$ and is subset of $A\times B$
### Graph of $R$:
- $A\times B$: [[Cartesian product]] of domain, set $A$, and codomain, set $B$. 
### Types of relation:
1. Reflexive:
	- if $(x,x)\in R$ for all $x\in S$
		- 10 mod 3 = 10 mod 3
		- every point has a path to itself
2. Symmetric:
	- if whenever $(x,y)\in R$ then $(y,x)\in R$
		- x → y and y → x
		- $xRy\to yRx$
		- Every path has a reverse path​
3. Transitive:
	 - whenever $(x,y)\in R, (y,z)\in R$ and $(x,z)\in R​$
		 - - x → y → z and x → z
		- every 2-step path has a 1-step path
### [[Math/Discrete/2. Functions and relations/Function]]
### Inverse relation:
- The inverse, $R^{-1}$ of a relation $R: A\to B$ is the relation from $B$ to $A$ defined by the rule $b\ R^{-1} \ a\iff a\ R\ b$