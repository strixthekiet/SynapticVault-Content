---
tags:
  - Math/linear/vector
---
# Orthogonality, Orthogonal Vectors
### Description:
- 2 n-vectors are orthogonal if $x^Ty=0\to x\perp y$
- Non zero vectors are said to be mutually orthogonal if each vector is orthogonal to all other vectors
	- they are also [[Vector#Vector Linear Independence|linearly indepent]]
### Orthonormal:
- A collections of vectors $S=\{ x^{(1)}, ...,x^{(d)}\}$ is said to be orthonormal if for $i,j=1,...d$
	- $\big(x^{(i)}\big) ^T x^{(j)} = \begin{cases} 0 &\text{if } i\not = j \\ 1 &\text{if } i=j \end{cases}$, meaning they are all unit vectors
- In words, $S$ is orthonormal if every element has unit norm, and all elements are orthogonal to eachother
- A collection of orthonormal vectors $S$ form an **orthonomal basis** for the span of $S$