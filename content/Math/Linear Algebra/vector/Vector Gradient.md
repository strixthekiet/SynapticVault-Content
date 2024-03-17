---
tags:
  - Math/linear/vector
aliases:
  - Gradient
---
# Vector Gradient
### Description:
- The gradient of a function $f :\mathbb R^n \to \mathbb R$ at a point $x$ where $f$ is differentiable, denoted with $∇f (x)$, is a column vector of first derivatives of $f$ with respect to $x_1, . . . , x_n$:
	- $\displaystyle ∇f (x)=\bigg[ \frac{\partial f(x)}{\partial x_1}    \ ...\ \frac{\partial f(x)}{\partial x_n}  \bigg]^T$ 
- The gradient of an [[Affine Function]] is $a$
### Geometric Interpretation:
- ![](https://www.math.net/img/a/calculus/vectors/gradient/gradient.png)
- The gradient of a [[Vector Function]] can be interpreted in the context of the level and sublevel sets.
- The $\alpha$-level set of a function $f\ : \ \mathbb R^n\to \mathbb R$ is the set $\{ x\in \mathbb R^n\ : \ f(x)=\alpha\}$
	- ie, the contours
	- and the $\alpha$-sublevel set is $\{ x\in \mathbb R^n\ : \ f(x)\le \alpha\}$
- Geometrically, the gradient of $f$ at a point $x_0$ is a vector $∇f (x_0)$ perpendicular to the contour line of $f$ at level $α = f (x_0)$, pointing from $x_0$  **outwards the $\alpha$-sublevel set** 
- That is, the gradient, $\nabla f(x_0)$ represents the direction along which the function has the max rate of increase
- Let $v$ be a unit vector and $\epsilon\ge 0$
- Consider the point $x=x_0+\epsilon.v$. We have $f(x_0+\epsilon.v)\approx f(x_0)+\epsilon. \nabla f(x_0)^T v$  for $\epsilon \to 0$
	- equivalently, $\displaystyle \lim_{\epsilon\to 0} \frac{f(x_0+\epsilon v)-f(x_0)}{\epsilon}=\nabla f(x_0)^Tv$
	- Think of it as the gradient projecting on the vector $v$
- Whenever $\epsilon> 0$ and $v$ is such that $\nabla f(x_0)^Tv>0$ then $f$ is increasing along the direction $v$, for small $\epsilon$??
- The inner product $\nabla f(x_0)^Tv$ measures the rate of variation of $f$ at $x_0$, along direction $v$, and it is usually referred to as the **directional derivative of $f$ along $v$**???
### Minimization via Gradient Descent Method:
- To solve an optimization problem of the form $\min\limits_x f(x)$ 
	- where $f$ is differentiable
- Start from $x_0$, iterate the rule $x_{k+1}=x_k - \alpha \nabla f(x_k)$
	- where $\alpha \gt 0$ is the step size
