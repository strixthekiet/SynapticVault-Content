---
mindmap-plugin: basic
tags:
  - Math/discrete/principle
---

# Well ordering principle

### Description:
- Every non-empty set of non-negative integers has a smallest element
### Claims:
- Any positive integers $m$ and $n$, fraction $\frac mn$ can be written in lowest term #Math/discrete/claim
	- Proof:
		- Suppose to the contrary that there are positive integers m and n such that the fraction m/n cannot be written in lowest terms.
		- Now let C be the set of positive integers that are numerators of such fractions. Then m ∈ C, so C is nonempty.
		- Therefore, by Well Ordering, there must be a smallest integer, m0 ∈ C. By definition of C, there exists n0 > 0 such that “the fraction m0/n0 cannot be written in lowest terms”
		- That is, m0 and n0 must have a common prime factor, p > 1. We have, $\frac{m_o/p}{n_0/p}=\frac mn$ , cannot be written in lowest terms either (by our assumption).
		- Therefore, m0/p ∈ C. But m0/p < m0, which contradicts the fact that m0 is the smallest element of C.

### Theorem:
- Every positive integer greater than one can be factored as a product of primes. #Math/discrete/theorem
- For any nonnegative integer, n, the set of integers greater than or equal to $−n$ is well ordered. #Math/discrete/theorem
- A lower bound (respectively, upper bound) for a set, S, of real numbers is a number, b, such that $b \le s$ (respectively, $b ≥ s$) for every $s ∈ S$. #Math/discrete/theorem
- Any set of integers with a lower bound is well ordered. #Math/discrete/theorem
