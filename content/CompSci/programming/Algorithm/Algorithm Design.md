---
tags:
  - CompSci/programming/Algorithm
---
# Algorithm Design
### Description:
- 
### Steps:
1. Formulate the problem precisely
2. Design an algo rithm
3. Prove the algorithm is correct
4. Analyze its runtime
### Algothrm design techniques:
- [[Greedy Algorithm]]
- [[Divide and Conquer]]
- [[Dynamic Programming]]
- [[Network Flow]]
### Complexity:
- An algorithm is efficient if its running time is a polynomial in the input size $T$
	- The running time is upper bounded by $c.T^d$ for some constants $c,d>0$
	- ex: brute force can solve Gale Shapley Algorithm in $n!$
- 2 main complexities:
	- [[Time Complexity]]
	- [[Space Complexity]]
### Algorithm's running time:
- To measure a [[Efficient Algorithm]]
- $f(n)$ is asymptotically bounded by $g(n)$
	- if $g(n)$ is asymptotically upper bound: [[Big O Notation]]
	- if $g(n)$ is asymptotically lower bound: [[Big Omega Notation]]
	- if $g(n)$ is asymptotically tight bound: [[Big Theta Notation]]
- Propositions:
	1. if $\displaystyle \lim\limits_{n\to\infty}\frac {f(n)}{g(n)}=c$ for some constant $c>0$ then $f(n)=\Theta(g(n))$
		- Proof: $c-\epsilon\le \frac{f(n)}{g(n)}\le c+\epsilon$ by definition
		- $(c-\epsilon)g(n)\le f(n)\le (c+\epsilon)g(n)$
		- by definition of Big Theta notation, it is true
	2. if $\displaystyle \lim\limits_{n\to\infty}\frac {f(n)}{g(n)}=0$ then $f(n)={\color{tomato}O}(g(n))$
	3. if $\displaystyle \lim\limits_{n\to\infty}\frac {f(n)}{g(n)}=\infty$ then $f(n)={\color{tomato}\Omega}(g(n))$
- To find which notation a function belongs to, do $\frac{f(n)}{g(n)}$
### Some classes of function:
- Polynomials:
	- $f(n)=\sum^d_{k=0} a_kn^k=O(n^d), a_d>0$
	- as $\displaystyle\lim_{n\to\infty}\frac{f(n)}{n^d}=a_d>0$
- Logarithms:
	- $\log_a(n)=\Theta(\log_b n)$ for every $a>1$ and $b>1$
	- as $\displaystyle\lim_{n\to\infty}\frac{\log_an}{\log_b n}=\frac 1 {\log_b a}=c$
- Logarithms and Polynomials:
	- $\log_a n=O(n^d)$ for every $a>1$ and every $d>0$
	- as $\displaystyle\lim_{n\to\infty}\frac{\log_a n}{n^d}=0$
- Exponentials:
	- $n^d=O(r^n)$ for every $r>1$ and every $d>0$
	- as $\displaystyle\lim_{n\to\infty}\frac{n^d}{r^n}=0$ 
- Factorials:
	- $n!=2^{\Theta(n\log n)}$
	- as by [[Stirling's Fomula]] $n!\approx\sqrt{2\pi n}(\frac re)^n$
---