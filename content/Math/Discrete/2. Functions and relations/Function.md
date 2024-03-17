---
mindmap-plugin: basic
tags:
  - Math/discrete
---
# Function:
### Definitions:
- $f:S\to T$ is a “mapping” from elements in set S to elements in set $T$
- $f$ is a relation on S and T such that for each $s\in S$, there exists a unique $t\in T$ such that $(s,t)\in R. \ S$ is the domain of f and T is range of $f$
- $\{ y \ | \ y=f(x)$ for some $x\in S\}$ is the image of f
- 1 x can only have 1 corresponding y
### Types of function:
- [[Injective function]]
- [[Surjective function]]
- [[Bijective Function]]
### Composition function:
- For functions $f: A\to B$ and $g: B\to C$, the composite $g\circ f$, of $g$ with $f$ is defined be the function from $A$ to $C$ defined by the rule: $(g\circ f)(x)\triangleq g(f(x))$
### Identity function of a [[Set|set]]:
- The identity function of a set $A$(written $\text{id}_A$ or just $\text{id}$) is the function $\text{id} :A\to A$ given by $\text{id}_A(x)=x$ (for all $x\in A$)
### Left inverse:
- $f\circ g=\text{id}$, then $f$ is the left inverse of $g$, and $g$ is the right inverse of $f$
### Right inverse:
-  $f\circ g=\text{id}$, then $g$ is the right inverse of $f$
### Two sided inverse:
- If $f$ is both a left- and a right-inverse of $g$, then $f$ and $g$ are two-sided inverses (of each other)
### Total function:
- The function $f$ from $A$ to $B$ is total when $f(x)$ exists for all $x\in A$
### Claims:
- $f$ is [[Injective function|injective]] and [[#Total function|total]] if and only if $f$ has a [[#Left inverse|left inverse]]. #Math/discrete/claim 
- $f$ is [[Surjective function|surjective]] if and only if $f$ has a [[#Right inverse|right inverse]] #Math/discrete/claim 
- $f$ is [[Bijective Function|bijective]] and [[#Total function|total]] if and only if $f$ has a two-sided inverse. #Math/discrete/claim 
### [[Set theory#5. Cardinality $ S $|Set cardinality]]:
- Let $S$ and $T$ be two potentially [[Set theory#6. A set can be infinite|infinite sets]]
	- $S$ and $T$ have the same cardinality, written as $|S|=|T|$, if and only if there exists a [[Bijective Function|bijection]] $f:S\to T$
	- $T$ has [[Set#Set cardinality|cardinality]] at larger or equal to $S$, written as $|S|\le |T|$, if and only if there exists an [[Injective function|injection]] $g:S\to T$ 
		- equivalently, if and only if there exist a [[Surjective function|surjection]] $g':T\to S$
### Countable [[Set|set]]: #Math/discrete/definition 
- A [[Set|set]] S is countable if it is finite or has the same [[Set#Set cardinality|cardinality]] as $\mathbb N^+$.
- Equivalently, $S$ is countable if $|S|\le|N^+|$
---