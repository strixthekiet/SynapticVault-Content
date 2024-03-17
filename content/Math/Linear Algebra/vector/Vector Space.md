---
tags:
  - Math/linear/vector
---
# Vector Space, $\chi$
### Description:
- Obtained by equipping [[Vector|vectors]] in a certain dimension with their [[Linear Combination]]
	- ie, the possible space that the vectors can be
### Properties:
- Closure under addition: 2 vectors adding cant escape the vector space
- Closure under scalar multiplication: 2 vectors multiply cant escape
### Basis of a vector space:
- A set of least [[Vector#Vector Linear Independence|linearly independent vectors]] that [[Span]] the full space
	- ie, n vectors that will let it span the whole subspace
	- ex, basis vector of a line is 1 vector; basis vectors of a plane are 2 vectors
- If we have a basis $\{x^{(1)},...,x^{(m)}\}$ for a subspace, $S$, then we can **uniquely** write any element in the subspace as a [[Linear Combination]] of elements in that basis.
	- That is, any $x\in S$ can be written as $\displaystyle x=\sum^d_{i=1} \alpha_i x^{(i)}$, for an appropriate $\alpha$
- To prove:
	- 2 conditions 
---