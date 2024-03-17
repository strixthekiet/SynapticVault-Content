---
mindmap-plugin: basic
tags:
  - Math/calculus/derivative
aliases:
  - partial derivative
---
# Partial derivative
### Description:
- [[Differentiation]] respect to multiple variables
### Functions of several variables: $z=f(x,y)$
- $\displaystyle \{ f(x,y)|(x,y)\in D\}$
- Graph:
	- Draw $f(x,y)=6-3x-2y$
		- Then let $z=f(x,y)$
		- Use quadric surface to draw $\to 3x+2y+z=6$
- Level curve:
	- Contour map consists of many level curves for $k=a,b,c,..$ would be the curve that represents all the points in the function where  $f(x,y) = a\text{ and } f(x,y)=b\text{ and }f(x,y))=c$
- Functions of three or more variables:
	- $D=f(x,y,z)$
	- 4-dimensional shape
### Limits and continuity:
- Find limit of $\lim\limits_{(x,y)\to{(a,b)}}f(x,y)$:
	- Approach from left side, $L_1=\lim\limits_{x\to 0}f(x,0)$
	- Approach from right side, $L_2=\lim\limits_{y\to 0}f(0,y)$
	- Approach from $y-b=m(x-a),\\L_3=\lim\limits_{x\to 0}f(x,m(x-a)+b)$
	- Approach from $y=x^2,L_3=\lim\limits_{x\to 0}f(x,x^2)$
	- Use different techniques to find limit
	- Limit exists all limits are the same
		- Be careful of the ridge
- $\lim\limits_{(x,y)\to{(a,b)}}f(x,y)=L$
- Continuity:
	- A polynomial function of two variables sum of terms in form of $cx^my^n$
		- is a continuous function
	- A rational function ratio of 2 polynomial
		- is a continuous function if denominator is not 0
	- Continuous function’s limit can be found by direct substitution
	- If $f(x,y)$ and $g(t)$ are both continuous then $h(x, y)= g(f(x, y))$ is also a continuous function
### Partial derivatives: 
- $D_xf=f_x(a,b)=g'(a)$
	- Partial derivative of $f$ with respect to $x$ at $(a, b)$, where $g(x)=f(x,b)$
		- Represent the tangent line where $y=b$
	- Regard $y$ as a constant, then function of $x,y$ becomes function of $x$
	- Same for $y$
		- $f_y(a,b)=h'(a)$ where $h(y) = f(a,y)$
	- Differentiate implicitly but for 3 variables
- $\displaystyle g'(a)= f_x(x,y)=\lim\limits_{h\to 0}\frac{g(x+h)-g(x)}{h}=\\\lim\limits_{h\to 0}\frac{f(x+h,y)-f(x,y)}{h}$
- Functions with more than 2 variables:
	- Treat the other 2 variables as constants
		- ex: $f(x,y,z)=e^{xy}\ln z\implies f_x=ye^{xy}\ln z$
- Higher derivatives:
	- $\displaystyle (f_x)_x=f_{xx} =f_{11}=\frac{\partial }{\partial x}\bigg(\frac{\partial f}{\partial x}\bigg)=\frac{\partial ^2f}{\partial x^2}=\frac{\partial ^2z}{\partial x^2}$
		- Differentiate $f_x$ in term of $x$ again
	- $\displaystyle (f_x)_y=f_{xy} =f_{12}=\frac{\partial }{\partial y}\bigg(\frac{\partial f}{\partial x}\bigg)=\frac{\partial ^2f}{\partial y\partial x}=\frac{\partial ^2z}{\partial y\partial x}$
		- Differentiate $f_x$ in term of $y$ again
	- $f_xy(a,b)=f_yx(a,b)$
- Partial differential equation:
	- Express certain physical laws
		- like Laplace equation $(u_{xx}+u_{yy}=0)$
		- and wave equation $(u_{tt}=a^2u_{xx})$

### Tangent planes and linear approximations:
- Tangent planes:
	- Let $C_1$ and $C_2$ be curves obtained by intersecting vertical lines $y=y_0$ and $x=x_0$
	- Let $T_1$ and $T_2$ be tangent line to $C_1$ and $C_2$
	- $z=f(x,y)$ then the tangent plane at $P(x_0,y_0,z_0)$ is $\displaystyle z-z_0=f_x(x_0,y_0)(x-x_0)+f_y(x_0,y_0)(y-y_0)$
- Linear approximations:
	- Linearization: $L(x,y)=f(a,b)+f_x(a,b)(x-a)+f_y(a,b)(y-b)$
	- Linearization: $L(x,y,z)=f(a,b,c)+f_{x_1}(x-a)+f_{y_1}(y-b)+f_{z_1}(z-c)$
	- If the partial derivatives $f_x$ and $f_y$ exist near $(a,b)$ and are continuous at $(a,b)$ then $f$ is continuous at $f(a,b)$
- Differentials:
	- $\displaystyle dz=f_x(x,y)dx+f_y(x,y)dy=\frac{\partial z}{\partial x}dx+\frac{\partial z}{\partial y}dy$
- Functions of three or more variables:
	- $\displaystyle dw = \frac{\partial w}{\partial x}dx+\frac{\partial w}{\partial y}dy+\frac{\partial w}{\partial z} dz$

### The chain rule:
- Case 1 (simple parametric):
	- $z=f(x,y)$ is a differentiable function and $x=g(t),y=h(t)$ are both differentiable $\displaystyle \implies\frac{dz}{dt}=\frac{\partial z}{\partial x}\frac{dx}{dt}+\frac{\partial z}{\partial y}\frac{dy}{dt}$
- Case 2 (two variable parametric):
	- $z=f(x,y)$ is a differentiable function and $x=g(s,t),y=h(s,t)$ are both differentiable
		- $\displaystyle \implies\color{tomato}\frac{\partial z}{\partial s}=\frac{\partial z}{\partial x}\frac{\partial x}{\partial s}+\frac{\partial z}{\partial y}\frac{\partial y}{\partial s}$
		- $\displaystyle \implies\color{tomato}\frac{\partial z}{\partial t}=\frac{\partial z}{\partial x}\frac{\partial x}{\partial t}+\frac{\partial z}{\partial y}\frac{\partial y}{\partial t}$
	- $s,t$ are independent variables; $x,y$ are intermediate variables; $z$ is dependent variables
- General version:
	- $\displaystyle \frac{\partial w}{\partial u}=\frac{\partial w}{\partial x}\frac{\partial x}{\partial u}+\frac{\partial w}{\partial y}\frac{\partial y}{\partial u}+\frac{\partial w}{\partial z}\frac{\partial z}{\partial u}+\frac{\partial w}{\partial t}\frac{\partial t}{\partial u}+...$
	- $\displaystyle \frac{\partial w}{\partial v}= \frac{\partial w}{\partial x}\frac{\partial x}{\partial v}+\frac{\partial w}{\partial y}\frac{\partial y}{\partial v}+\frac{\partial w}{\partial z}\frac{\partial z}{\partial v}+ \frac{\partial w}{\partial t}\frac{\partial t}{\partial v}+...$
	- same for more independent variables
- Implicit differentiation $F(x,y)=F(x,fx)=0$:
	- Case 1:
		- Suppose that $y$ is given implicitly as a function by an equation $y=f(x)$ by equation of the form $F(x,y)=F(x,f(x))=0$
			- $\displaystyle \implies \color{tomato}\frac{dy}{dx}=-\frac{F_x}{F_y}$
	- Case 2:
		- Suppose that $z$ is given implicitly as a function by an equation $z=f(x,y)$ by equation of the form $F(x,y,z)=F(x,y,f(x,y))=0$
			- $\displaystyle\implies \frac{\partial z}{\partial x}=-\frac{\partial F} {\partial x}\bigg/\frac{\partial F} {\partial z}=\color{tomato}-\frac{F_x}{F_z}$
			- $\displaystyle\implies \frac{\partial z}{\partial y}=-\frac{\partial F} {\partial y}\bigg/\frac{\partial F} {\partial z}=\color{tomato}-\frac{F_y}{F_z}$
### Directional derivatives & the gradient vector:
- $\displaystyle D_uf(x_0,y_0)=\lim\limits_{h\to 0}\frac{f(x_0+ha,y_0+hb)-f(x_0,y_0)}{h}=\color{tomato}\nabla f({\bf x}).\hat u$
- Directional derivative:
	- $\displaystyle D_uf(x_0,y_0)$ denote directional derivative $f$ at $(x_0,y_0)$ in the direction $u$
	- $f_x$ and $f_y$ are special cases of directional derivative:
		- $\displaystyle D_uf(x,y)=f_x(x,y).a+f_y(x,y).b\\ =f_x(x,y)\cos\theta+f_y(x,y)\sin\theta$
			- bcz $a={\bf u}\cos\theta$
			- where $\theta$ is the angle $\bf u$ makes with $x$-axis
- Gradient vector : $\displaystyle \nabla f(x,y)$
	- Gives the direction of fastest increase of $f$
	- also the directional of the line orthogonal to the level surface $S$ of $f$ through $P$
	- also the perpendicular line to the level curve $f(x,y)=k$
	- By dot product: $\displaystyle D_uf(x,y)=f_x(x,y).a+f_y(x,y).b\\= \underbrace{\langle f_x(x,y)+f_y(x,y)\rangle}_{\nabla f(x,y)}\cdot {\bf u}$
	- Gradient vector: $\displaystyle {\color {tomato} \nabla f(x,y)=\langle f_x,f_y\rangle}=\frac{\partial f}{\partial x}{\bf i}+\frac{\partial f}{\partial y}{\bf j}$
- Functions of three variables:
	- Directional vector
		- $\displaystyle D_uf(x,y,z)=f_x(x,y,z).a+f_y(x,y,z).b+f_z(x,y,z).c\\= \nabla f(x,y,z)\cdot {\bf u}$
	- Gradient vector represents the normal line pokes perpendicular through the surface
		- $\displaystyle\nabla f(x,y,z)=\langle f_x,f_y,f_x\rangle=\frac{\partial f}{\partial x}{\bf i}+\frac{\partial f}{\partial y}{\bf j}+\frac{\partial k}{\partial y}{\bf k}$
- Maximizing the directional derivative:
	- The maximum value of the directional derivative is $D_{\bf u}f({x,...}) \text{ is } \color{tomato}|\nabla f({x,...})|$
		- occurs when $\bf u$ is the unit vector of gradient vector $\nabla f({x,...})$
- Tangent planes to level surfaces:
	- Tangent plane:
		- Let $x,y,z$ be functions of $\displaystyle t\\\to F(x(t),y(t),z(t))=k\\ \to \frac{\partial f}{\partial x}\frac{dx}{dt}+\frac{\partial f}{\partial y}\frac{dy}{dt}+\frac{\partial k}{\partial y}\frac{dz}{dt}=\nabla F\cdot {\bf r}'(t) =0\\ \to\color{tomato} F_{x0}(x-x_0)+F_{y0}(y-y_0)+F_{z0}(z-z_0)=0$ is the equation of tangent plane to the level surface $F(x,y,z)=k$ at $P(x_0,y_0,z_0)$
	- Symmetric equations of normal line to S at P:
		- $\displaystyle\color{tomato} \frac{x-x_0}{F_x}=\frac{y-y_0}{F_y}=\frac{z-z_0}{F_z}$
### Maximum and minimum values:
- Absolute minimum/maximum value:
	- $\nabla f(a,b)=f_x(a,b)=f_y(a,b)=0$ then $(a,b)$ is critical point
- Second derivatives test:
    
	- $D=\begin{vmatrix} f_{xx} & f_{xy} \\ f_{yx} & f_{yy} \end{vmatrix}=\color{tomato}f_{xx}f_{yy}-(f_{xy})^2$
	
	1. $\color{tomato}D>0$ and $\color{tomato}f_{xx}>0$ then $f(a,b)$ is a local minimum
	2. $\color{tomato}D>0$ and $\color{tomato}f_{xx}<0$ then $f(a,b)$ is a local maximum
	3. $\color{tomato}D<0$ then $f(a,b)$ is not a local maximum or minimum, it is a saddle point
		- $f$ is maximum in $x$ direction but minimum in $y$ direction or vice versa
- Closed set vs bounded set
- Extreme value theorem for functions of two variables:
	- If $f$ is continuous on a closed, bounded set $D$ in $\mathbb R^2$, then $f$ attains an absolute max value $f(x_1,y_1)$ and an absolute min value $f(x_2,y_2)$ at some points in $D$
- To find absolute max and min for bounded set:
	1. Find the values of $f$ at the critical points of $f$ in $D$
	2. Find the extreme values of $f$ on the boundary
		- when $x=x_{min}/x_{max}$ and $y=y_{min}/y_{max}$
	3. Compare the values
### Lagrange multipliers:
- To find the maximum and minimum values of $f(x,y,z)$ subject to the constraint $g(x,y,z)=k$
	1. Find sets of values of $x,y,z$ and $\lambda$ such that:
		- $\color{tomato}\nabla f(x,y,z)=\lambda \nabla g(x,y,z)$
			- same tangent line in the level curves
		- $g(x,y,z)=k$
	2. Evaluate all points from(a). The largest of these values is the maximum value of $f$
- For two constraints:
	- To find the max and min values of $f(x,y,z)$ subject to the constraints $g(x,y,z)=k$ and $h(x,y,z)=l$
		- $\color{tomato}\nabla f(x,y,z)=\lambda \nabla g(x,y,z)+\mu \nabla h(x,y,z)$
		- $g(x,y,z)=k$
		- $h(x,y,z)=l$
