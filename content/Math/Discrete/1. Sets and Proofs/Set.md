---
mindmap-plugin: basic
tags:
  - Math/discrete/definition
  - Math/statistic
aliases:
  - set
  - sets
---

# Set

## Definition
- An unordered collection of distinct objects (elements)
- A set is said to contain its elements.
	- Set with no element is empty set or null set
	- A set with one element is called a singleton set
- We write $a\in A$ to denote that $a$ is an element of the set $A$
	- For every set, $\emptyset\subseteq S$ and $S\subseteq S$   #Math/discrete/theorem ^77bf1e

## Ways to specify a set:
- set roster: $\{a,b,c\}$
- set builder notation: $P=\{ x\in \mathbb Z^+| x \text{ is prime nb and }x < 20 \}$: $x \in \mathbb Z^+$ such that ...
- Popular sets

## Popular sets:
- $(\mathbb{Q}=\{ p/q\ |\ p\in \mathbb Z,\ q\in \mathbb Z,\ \text{and } q\not= 0\})$
- | Natural | Integer | Positive int | Rational | Real | Positive Real | Complex |
| --- | --- | --- | --- | --- | --- | --- |
| $\mathbb N$ | $\mathbb Z$ | $\mathbb Z^+$| $\mathbb{Q}$ | $\mathbb R$ | $\mathbb R^+$| $\mathbb{C}$|

## Equal sets: $A=B$ #Math/discrete/definition
- Two sets are equal if and only if they have the same elements.
	- We write $A = B$ if $A$ and $B$ are equal sets.

## Subset: $A\subset B$ #Math/discrete/definition
- A is subset of B, B is super set of A $(B\supseteq A)$
	- $A\subset B$: proper subset, when $A\not = B$
	- if $A\subseteq B$ and $B\subseteq A\implies A=B$

## Set cardinality:$|S|$  #Math/discrete/definition
- $|S|$: non-negative integer denotes exact number of element for a ==finite set== S
	- 1. $|S| = n\to|P(S)|=2^n$

## Infinite set: #Math/discrete/definition
- A set is said to be infinite if it is not finite

## Power sets: $\mathcal P(S)$ #Math/discrete/definition
- power set of S is set of all subsets of set S, e.g. $\mathcal{P}({1,2})=\big\{ \emptyset, \{1\}, \{2\}, \{1,2\} \big\}$
	- $\mathcal{P}(\emptyset)=\{\emptyset\}$
	- $\mathcal{P}(\{\emptyset\})=\{ \emptyset, \{\emptyset\} \}$
	- every subset of a set is an element in its power set

## Set operations:
- Union operation
- Intersect operation
- Difference operation
- Complement operation