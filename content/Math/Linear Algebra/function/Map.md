---
tags:
  - Math/linear/vector
---
# Map
### Description:
- Refer to vector-valued functions
- Maps are [[Vector Function|linear function]]s that return a vector of value instead of 1 value
	- $f\ : \ \mathbb{R}^n \to \mathbb R^m$
- The components of the map $f$ are scalar-valued functions $f_i$ for $i=1,2,...,m$
### Sets related to functions:
- Graph:
	- Consider [[Vector Function|function]] $f:\mathbb R^n: \mathbb R$
	- The **graph** of $f$ is the set of input-output pairs that $f$ can attain
		- with $f(x)$ as the $n+1$ element of the vector
	- graph $f=\ \big\{ (x,f(x))\in \mathbb{R}^{n+1}: x\in \mathbb{R}^n    \big\}$ 
- Level set, or contour line:
	- The set of points that achieve exactly some value for the function $f$
	- For $t\in\mathbb R$, the $t$-level set of the function $f$ is defined as:
		- $C_f(t)=\big\{ x\in \mathbb R^n:\ \ f(x)=t    \big\}$ but typically only take 2 $x(i)$ to graph
		- ![](https://r-charts.com/en/correlation/contour-plot_files/figure-html/contour-nlevels.png)
	- The **$t$-sublevel** set of $f$ is the set of points that achieve at most a certain value for $f$:
		- $L_f(t):\big\{x\in \mathbb R^n \ : \ f(x)\le t \big\}$ 