---
tags:
  - Math/linear/vector
---
# Visualizing Data by Projection
### Description:
- We can visualize the data set that each data point has a vector, by projecting each data point on  a one-, two- or three-dimensional space. 
	- Each “view” corresponds to a particular projection on a direction
- In the 1D case, the projection on a given line passing through $x^0$ and direction $a$ is related to a scoring function, of the form $f : x → a^T x + b$ where $x ∈ \mathbb R^n$ is a data point, and $a ∈ \mathbb R^n, b ∈ R$ are given.  
	- WLOG we can set $||a||_2 = 1$ 
### Centering:
- We can center the scores so that the average score across data points is zero, that is:
	- $\displaystyle  0= \frac 1m \sum^m_{i=1} f(x_i)=\frac 1m \sum^m_{i=1} (a^T x_i +b)=a^T \hat x +b$ 
- This implies a condition on $b:b = −a^T \bar x$, where $\displaystyle \hat x := \frac 1 n\sum ^n_{i=1} x_i\in \mathbb R^n$ is the center of the points for that $a$ projection
- Then we can adjust the scoring function to be $f (x) = a^T (x − \hat x)$
- Equivalently we project the **centered** data points on a line passing through $0$