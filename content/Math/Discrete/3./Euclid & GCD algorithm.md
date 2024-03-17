---
mindmap-plugin: basic
tags:
  - Math/discrete/definition
---
# Euclid & GCD algorithm
### Description:
- 
  ```python
  def EuclidAgl(a,b):
	  if b = 0:
		  return a
	  else:
		  return EuclidAlg(b, a mod b)
	```
	- If $a,b\in \mathbb N, b\not=0$ then $gcd(a,b)= gcd(b, a\mod b)$ #Math/discrete/lemma
- Euclid’s algorithm, on input EuclidAlg(a, b) for $a, b ∈ N^+, a, b$ not both 0, always terminates and produces the correct output. #Math/discrete/theorem 
- For every two recursive calls made by EuclidAlg, the first argument a is at least reduced by halved. #Math/discrete/claim 
- Euclid’s algorithm, on input EuclidAlg(a, b) for$ a, b ∈ N+, a, b$ not both 0, always terminates in time proportional to $log_2 a$. #Math/discrete/theorem 
