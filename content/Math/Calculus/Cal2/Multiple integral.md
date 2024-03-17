---
mindmap-plugin: basic
tags:
  - Math/calculus/integral
  - Math/statistic
---
# Multiple integral
### Double integrals over rectangles:
- $R=[a,b]\times[c,d]=\big\{\{x,y\}\in \mathbb R ^2|a\le x\le b, c\le y\le d\big\}$
### Double integrals over general regions:
- When $F(x,y) = \begin{cases} f(x ,y)&\text{if } (x,y) \text{ is in } D \\ 0 &\text{if }(x,y) \text{ is in R, not in } D \end{cases}$
	- Discontinuous on the boundary of $D$
	- Choose type 1 or 2 for easy integration
	- Type I: $y=g(x)$
		- $D=\bigg\{ (x,y)|a\le x\le b, g_1(x)\le y\le g_2(x)\bigg\}$
		- $\displaystyle V=\color{tomato}\int ^b_a\int^{{\color{green}g_2(x)}}_{{\color{green}g_1(x)}} f(x,y).{\color{green}dy}.dx$
		- Integral that is first evaluated is always the function
    - Type II: $x=h(y)$
	    - $D=\bigg\{ (x,y)|c\le y\le d, h_1(y)\le x\le h_2(y)\bigg\}$
	    - $\displaystyle V=\color{tomato}\int ^d_c\int^{h_2(y)}_{h_1(y)} f(x,y).dx.dy$
- Convert between 2 types: draw the area and reverse roles
- Properties of double integral:
    - $\displaystyle \int\int_D f(x,y)dA=\int\int_{D_1}f(x,y)dA+\int\int_{D_2}f(x,y)dA$
---
### Triple integrals:
- Triple integral of $f$ over the box $B=[a, b]\times[c,d]\times[r,s]$ is
	- $\displaystyle \int\int\int_B f(x,y,z)dV=\int ^s_r\int^d_c\int^b_af(x,y,z)dx.dy.dz$
	- Any of the six possible order of integration works
	- Use polar whenever there is circle involved
- Triple integral over a general bounded region $E$
	- Outside is independent, middle depends on outside and inside depends on both (or one)
	- Type I: $y=g(x)$ and $x=h(y)$
		- $E=\{(x,y,z)|(x,y)\in D,u_1(x,y)<z<u_2(x,y)\}$
		- Projection of E is D onto $xy$ plane
		- $\displaystyle V=\int ^b_a\int^{{\color{tomato}g_2(x)}}_{{\color{tomato}g_1(x)}} \int^{u_2(x,y)}_{u_1(x,y)}f(x,y,z){\color{tomato}dz.dy}.dx\\=\int ^d_c\int^{{\color{tomato}h_2(y)}}_{{\color{tomato}h_1(y)}} \int^{u_2(x,y)}_{u_1(x,y)}f(x,y,z){\color{tomato}dz.dx}.dy$
	- Type II: $x=u(y,z)$
		- $E=\{(x,y,z)|(y,z)\in D,u_1(y,z)<x<u_2(y,z)\}$
		- Projection of E is D onto $yz$ plane
		- $\displaystyle V =\int\int_D \bigg[ \int^{{\color{tomato}u_2(y,z)}}_{{\color{tomato}u_1(y,z)}} f(x,y,z) dx\bigg]dA$
	- Type III: $y=u(x,z)$
		- $E=\{(x,y,z)|(x,z)\in D,u_1(x,z)<y<u_2(x,z)\}$
		- Projection of E is D onto $xz$ plane
		- $\displaystyle V =\int\int_D \bigg[ \int^{{\color{tomato}u_2(x,z)}}_{{\color{tomato}u_1(z,z)}} f(x,y,z) dy\bigg]dA$
- Remember that the limits of integration in the inner integral contain at most two variables, the limits of integration in the middle integral contain at most one variable, and the limits of integration in the outer integral must be constants.
