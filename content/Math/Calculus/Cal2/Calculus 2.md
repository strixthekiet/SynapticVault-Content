---
Credits: 4
Done: true
---
$$ \text{Chapter 9: Paramatric equation and polar coordinates} $$

## Parametric curves: $(x,y)=(f(t),g(t))$

- $x=f(t), y=f(t)$ for $a<t<b$
    
    - Then there are initial point $(f(a),g(a))$ and terminal point $(f(b),g(b))$
    - We can graph $x=g(t)$ and $y=t$ by graphing $x=g(y)$
        - eg. $x=\sin^2t, y=\sin t\implies x=y^2$
- Cycloid:
    - Let the parameter be $\theta$
    - $|OT| = \text{arc}PT=r.\theta$
    
    $\implies x=|OT|-|PQ|=r.\theta-r.\sin\theta$
    
    $\implies y=|CT|-|CQ|=r-r.\cos\theta$
    

![Screenshot 2023-03-10 at 15.39.53.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/3cfc0667-9f19-4905-8696-895605ee3d57/Screenshot_2023-03-10_at_15.39.53.png)

## Calculus with parametric curves:

- Tangent:
    
    - By chain rule, $\displaystyle \frac {dy}{dx}=\frac{dy/dt}{dx/dt}$ when $dx/dt \not= 0$
    - $\displaystyle \frac {d^2y}{dx^2}=\frac{d(\frac{dy}{dx})}{dx}=\frac{d(dy/dx)/dt}{dx/dt}$
- Area under graph:
    
    - $y=g(t)$ and $dx=f'(t)dt$
    - $a$ is $t$ of the leftmost point which has minimum $x$

![Screenshot 2023-02-28 at 19.05.25.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/6f6471af-369b-43fb-a3e3-dce18e743920/Screenshot_2023-02-28_at_19.05.25.png)

- Arc length:
    - Curve _C_ is traversed exactly once as $t$ increases from $\alpha$ to $\beta$, then arc length is
        - If $t$ traverses twice then $L$ twice times the actual arc length

![Screenshot 2023-02-28 at 19.49.25.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/38874930-0ecd-473f-aacf-6ab95131ba27/Screenshot_2023-02-28_at_19.49.25.png)

$x=f(t), y=g(t),\alpha \le t\le\beta$ where $f'(t)$ and $g'(t)$ are continuous on $[\alpha,\beta]$,

## Polar coordinates: $(r,\theta)$

- $O$, The pole is the origin
- The ray(half-line) is drawn $\theta$ angle horizontally corresponds to the positive $x$-axis
    - $r$, the distance from $O$ can be negative
    - $\theta$ is the angle

![Screenshot 2023-02-28 at 13.22.47.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/938c769a-e9ad-4a66-ad9e-1457397d4d24/Screenshot_2023-02-28_at_13.22.47.png)

- Polar curve:
    - a collection of points satisfying $r=f(\theta)$
        - $x=r.\cos \theta$
        - $y=r.\sin\theta$
        - $r^2=x^2+y^2$
        - $\displaystyle \tan\theta=\frac yx$

![Screenshot 2023-02-28 at 13.31.39.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/932dbe9d-4fb5-4f36-99b0-cf5cfc31a576/Screenshot_2023-02-28_at_13.31.39.png)

- Tangent to polar curve:
    - Find the point where tangent is horizontal $\implies \frac{dy}{d\theta}=0$
        - Put $\theta$ and only take points where $r>0$

![Screenshot 2023-02-28 at 13.59.57.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/df489f80-d9a3-4683-8491-02263eacd6c1/Screenshot_2023-02-28_at_13.59.57.png)

## Area and lengths in polar coordinates:

- Area under graph:
    - Find area between 2 curves:
        - Find the intersection first, which are the limits
        - or cut the shape to parts in which each part is area under graph of 1 curve

$\displaystyle A=\int^b_a\frac12 r^2d\theta=\int^b_a\frac12 f^2(\theta)d\theta$

$\displaystyle A=\frac12 \bigg[\int^b_af^2(\theta)d\theta -\int^b_ag^2(\theta)d\theta\bigg]$

![Screenshot 2023-03-17 at 12.27.18.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/f26d7cad-8cc5-44b9-a194-67cf3a678fc8/Screenshot_2023-03-17_at_12.27.18.png)

- Arc length:
    - Distance traveled is difference

$\displaystyle L=\int^b_a\sqrt{{r}^2+\bigg( \frac{d{ r}}{d\theta}\bigg)^2}d\theta$

$$ \text{Chapter 10: Vectors and the geometry space} $$

## 3D coordinates systems:

- Equation of a sphere: $(x-h)^2+(y-k)^2+(z-l)^2=r^2$ where the centre is $C(h,k,l)$

![Screenshot 2023-03-13 at 17.17.03.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/c4206149-97b5-49a5-bf9c-5a99aa3ad0a6/Screenshot_2023-03-13_at_17.17.03.png)

## Vectors:

![Screenshot 2023-03-13 at 17.19.17.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/5dfb2635-6d8e-4d95-b1b1-d623df3c4f74/Screenshot_2023-03-13_at_17.19.17.png)

![Screenshot 2023-03-13 at 17.19.47.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/6531ac6e-8bdc-4c30-ade8-5685d4f73d62/Screenshot_2023-03-13_at_17.19.47.png)

## The Dot Product:

$$ ⁍ $$

- $\theta$ is the angle between the 2 vectors both pointing toward the intersection
    - Find $\angle ABC\implies \overrightarrow{AB}\cdot\overrightarrow{CB}$, both vectors are pointing toward B
    - $\pi-\theta$ to find the angle if 1 vector is pointing toward and the other is pointing away
    - Or change direction of 1 vector by inverting it or
- $a\cdot b=|a|.|b|.Cos90=0$ when 2 vectors are perpendicular
- $a\cdot b=|a|.|b|.Cos0=|a|^2$ when 2 vectors are parallel and have same direction
- $a\cdot b\cdot c$ has no meaning

## The Cross Product:

- Vector determinant:
    - results to another vector

$$ n=a\times b =\begin{vmatrix} \bold{i} & \bold{j} & \bf{k} \\ a_i & a_j & a_k \\ b_i & b_j & b_k \end{vmatrix} ; \text{note that} \color{tomato} \bold{-j} $$

![Screen Shot 2021-09-30 at 9.47.20 PM.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/ebfc8511-ed27-4d9b-b13a-cd1634c1876b/Screen_Shot_2021-09-30_at_9.47.20_PM.png)

![Screenshot 2023-03-06 at 10.54.44.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/e6cc2564-5d5d-4d68-9021-cc51436f2481/Screenshot_2023-03-06_at_10.54.44.png)

- if $\theta$ is the angle between $a$ and $b$ then: $\color{tomato}|a\times b|=|a|.|b|.\sin\theta$
- Right-hand rule:
    - If the fingers of your right hand curl in the direction of a rotation (through an angle less than 180) from $a$ ****to $b$, then your thumb points in the direction of $a\times b$

![Screenshot 2023-03-17 at 13.25.59.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/55542c31-dc21-41c7-872a-648b5748b82a/Screenshot_2023-03-17_at_13.25.59.png)

- Properties:
    - $a\times a=0$ for all $a\in V_3$
    - The vector $a\times b$ is orthogonal, common perpendicular, to both $a$ and $b$
    - Two non-zero vectors $a$ and $b$ are parallel if and only if $a\times b=0$

![Screenshot 2023-03-06 at 11.10.55.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/ae7c3bd7-ec5b-4be1-834a-2f678ee04a81/Screenshot_2023-03-06_at_11.10.55.png)

- The area of parallelogram is $\color{tomato}|a\times b|=|a|.(|b|.\sin\theta)$

![Screenshot 2023-03-13 at 18.01.06.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/abe72aa3-dc85-42d8-b856-a53d28b0ad30/Screenshot_2023-03-13_at_18.01.06.png)

- Triple products (scalar triple product):
    
    $a.(b\times c)=a\begin{vmatrix} a_i &a_j& a_k \\ b_i& b_j & b_k\\ c_i & c_j & c_k \end{vmatrix}$
    
    - Volume of parallelepiped:
        - $h=|a|.\cos\theta\\\implies V=|b\times c|.|a|.|\cos\theta | \\ V= |a.|b\times c||$

![Screenshot 2023-03-13 at 17.50.47.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/0759eefd-5fab-4244-8087-7770f053b886/Screenshot_2023-03-13_at_17.50.47.png)

## Equation of lines and planes:

- Find the line intersection of 2 planes:
    - Let one variable be free, $(z=t)$
    - Substitute in others 2 equations $(x=f(t),y=g(t))$
    - Split it to equation in term $r=(a,b,c)+\lambda(x,y,z)$

## Cylinders and quadric surfaces:

- Cylinders
    - Surface that consists of all lines (called **rulings**) that are parallel to a given line and pass through a given plane curve

![Screenshot 2023-03-06 at 11.23.02.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/16842a35-4e16-465b-a7e3-cafcb8fd50b8/Screenshot_2023-03-06_at_11.23.02.png)

$z=x^2$ to $(x,y,x^2)$

![Screenshot 2023-03-06 at 11.24.47.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/6ca40cc8-b57d-4aa5-877f-950970df51ec/Screenshot_2023-03-06_at_11.24.47.png)

$y^2+z^2=1$ to $(x,y^2,1-y^2)$

- Quadric surface
    - A second-degree equation in three variables x, y, and z
    - $Ax^2+By^2+Cz^2+J=0 \space \text{or}\space Ax^2+By^2+Iz=0$
    - Draw:
        - Let $z=k$, we have $x^2+(\frac{y}3)^2=1-\frac{k^2}4; (k^2<4)$
            
            which is many level curves of ellipse on $x-y$ plane at $(0,0)$ with 3 units in $y$-direction
            
        - Let $y=k$ then $x=k$
            

![Screenshot 2023-03-14 at 10.14.45.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/3f35bf73-99ba-44ff-9817-1f94cdd70f01/Screenshot_2023-03-14_at_10.14.45.png)

$x^2+\frac{y^2}9+\frac{z^2}4=1$

![Screenshot 2023-03-14 at 10.30.34.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/49c34ac0-861b-4e88-bdd2-8fd5215c5682/Screenshot_2023-03-14_at_10.30.34.png)

## Vector functions and space curves:

- Functions $fgh(t)$ are parametric equations
    
- As $t$ varies throughout the interval, it forms a space curve
    
    ${\bold r}(t)=\langle f(t),g(t),h(t)\rangle,$ then $\lim\limits_{t\to a} {\bold r}(t)=\langle \lim\limits_{t\to a}f(t), \lim\limits_{t\to a}g(t), \lim\limits_{t\to a}h(t)\rangle$
    
    Provides limits of the component functions exist
    
- A vector function $\bold r$ is continuous at $a$ if $\displaystyle \lim\limits_{t\to a}={\bold r}(a)$
    

![Screenshot 2023-03-17 at 13.44.35.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/df737d28-5d6b-45d5-8500-c963c468b834/Screenshot_2023-03-17_at_13.44.35.png)

A helix $\\\cos(t)+\sin(t)+t$

- Sketch:
    
    - $\langle t,2-t,2t\rangle \implies (0,2,0)+t(1,-1,2)$ thus a line
    - $\langle\cos(t),\sin( t) ,t \rangle \implies$
- Derivatives:
    
    $\displaystyle \frac{d{\bold r}}{d\theta}={\bold r}'(t)=\lim\limits_{h\to 0}\frac{{\bold r}(t+h)-{\bold r}(t)}{h}\\=f'(t)i+g'(t)j+h'(t)k$
    
    - Tangent vector of $\displaystyle {\color{tomato}\bold r} ={{\bold r'(t)}}$

![Screenshot 2023-03-17 at 14.25.49.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/e6c897bd-7783-4ce9-8030-ab8aacd7e32c/Screenshot_2023-03-17_at_14.25.49.png)

- Integral:

$\displaystyle \int^b_a {\bold r}(t)dt=\bigg(\int^b_af(t)dt \bigg)i+\bigg(\int^b_ag(t)dt \bigg)j +\bigg(\int^b_ah(t)dt \bigg)k+\color{tomato}C$

- $C$ is an arbitrary constant vector

## Arc length and curvature:

- Arc length:
    
    $\displaystyle L=\int^b_a |r'(t)|dt=\int^b_a\sqrt{\bigg( \frac{dx}{dt}\bigg)^2+\bigg( \frac{dy}{dt}\bigg)^2 +\bigg( \frac{dz}{dt}\bigg)^2}dt$
    
    - Note that $a$ and $b$ are from $t$
    - Distance traveled is difference

![Screenshot 2023-03-17 at 15.51.15.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/a387450c-2355-4e91-a78a-e3d13f72947a/Screenshot_2023-03-17_at_15.51.15.png)

- Parametrizations:
    
    - A single curve $C$ can be represented by more than one vector functions, they are parametrizations of curve $C$
        
        ![Screenshot 2023-03-17 at 16.24.44.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/532fdac8-e5bb-4e39-a277-8087af8287be/Screenshot_2023-03-17_at_16.24.44.png)
        
    - ex: $r_1(t)=\langle t,t^2,t^3\rangle, 1\le t\le 2$ is the same as $r_2(u)=\langle e^u,e^{2u},e^{3u}\rangle, 0\le u\le \ln2$
        
        - $t=e^u$
    - Thus, arc length is independent of the parametrization that is used
        
    - Parametrize a curve with respect to arc length
        
        - $r(t(s))$: to find the coordinates knowing the arc length
        
        1. Find $s(t)=L$, the arc length function
        2. $s=s(t)=\int^t_0|{\bold r}'(u)|du$
        3. substitute $t$ as function of $s$ in
- Curvature:
    
    - A parametrization ${\bold r}(t)$ is **smooth** on an interval I if **$\bold r$** is continuous and ${\bold r}(t)\not =0$ in I
        
    - Unit tangent vector:
        
    
    $\displaystyle\color{tomato} {\bold T}(t)=\frac{{\bold r'(t)}}{|{\bold r'(t)}|}$
    
    - Curvature of the curve:
    
    $\displaystyle {\color{tomato}\kappa} = \bigg| \frac{d{\bold T}}{ds} \bigg|=\bigg| \frac{d{\bold T/dt}}{ds/dt} \bigg|=\color{tomato} \frac{|{\bold T}'(t)|}{|{\bold r}'(t)|}$
    
    $\displaystyle\color{tomato} \kappa =\frac{|{\bold r}'(t)\times{\bold r}''(t)|}{|{\bold r}'(t)|^3}$ use this
    
    - For explicit equations: $y=f(x)$
    
    $\displaystyle \kappa = \color{tomato}\frac{|f''(x)|}{[1+(f'(x))^2]^{3/2}}$
    
- Normal and Binormal vectors:
    
    - Principal unit normal vector: $\color{tomato}\displaystyle{\bold N}(t)=\frac{{\bold T}'(t)}{|{\bold T}(t)|}$
        - Indication of which direction the curve is turning
    - Binormal vectors: $\color{tomato}{\bold B}(t)={\bold T}(t)\times{\bold N}(t)$
        - An unit vector, perpendicular to both $\bold T$ and $\bold N$

![Screenshot 2023-03-20 at 21.57.31.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/d76cfb57-7644-4439-abb5-efe1eb3852fa/Screenshot_2023-03-20_at_21.57.31.png)
### Chapter 11: [[Partial derivative]]

### Chapter 12: [[Multiple integral]]
$$ \text{Chapter 13:Vector calculus} $$

## Vector fields:

- Vector fields: ${\bold F}({\bold x})=f({\bold x})i+g({\bold x})j+h({\bold x})k$
    - $f(x,y,z)$ is a component function
    - For every point $({\bold x}_1)$ becomes $(f({\bold x})i,g({\bold x})j,h({\bold x})k)$ then ${\bold F}({\bold x})$ is a vector field

![ezgif.com-gif-to-webp.webp](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/1a37a44c-00f7-40b5-a42d-7880aa31ba95/ezgif.com-gif-to-webp.webp)

- Gradient fields: $\nabla f({\bold x})=f_x({\bold x})i+g_y({\bold x})j+h_z({\bold x})k$
    - Forms a gradient vector field
    - A vector field ${\bold F}$ is called a conservative vector field if there exists a function $f$ **such that ${\bold F}=\nabla f$
        - $f$ is a potential function of ${\bold F}$
        - Any path $C$ between two point have the same $\int_{C} F\cdotp d\bold r$ (like work done by gravity), a fluid flows back to where it was with same speed

![Screenshot 2023-05-15 at 11.33.59.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/57b5ad3d-3ed9-48b6-b39b-75865a431ffc/Screenshot_2023-05-15_at_11.33.59.png)

## Line integrals:

- Integral over a curve where $x=x(t),y=y(t), a\le t\le b$$x=x(t),y=y(t), a<t<b$
    
    - Equivalent to $\bold r (t)=x(t)\bold i+y(t)\bold j$
- $\color{tomato}\displaystyle \int_C f(x,y)ds =\int^b_a f\big(x(t),y(t)\big)\sqrt{
    

\bigg( \frac{dx}{dt}\bigg)^2+ \bigg( \frac{dy}{dt}\bigg)^2 }

dt$ - Use $x=\cos t,y=\sin t$ for circle

- $\int f(x,y)ds=\int_{C1} f(x,y)ds+\int_{C2} f(x,y)ds+...+\int_{Cn} f(x,y)ds$
    - Define domain of $t$ for each piece

![Screenshot 2023-05-23 at 13.47.32.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/b58c9643-3be8-4051-8e17-d990b58995d3/Screenshot_2023-05-23_at_13.47.32.png)

![Screenshot 2023-05-23 at 13.33.40.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/84345b6d-c92f-40c5-af2c-f5ef3174c751/Screenshot_2023-05-23_at_13.33.40.png)

- Applications are similar to double and triple integral
    
- Line integral with respect to $x$ or $y$:
    
    - Vector representation of a line starts at $\bold r_0$ ends at $\bold r_1$:
        - $\bold r(t)=(1-t)\bold r_0+t\ \bold r_1$ for $0\le t\le 1$
    - $\color{tomato}\displaystyle dx=x'(t) \to \int_Cf(x,y)dx=\int^b_af\big(x(t),y(t)\big).x'(t)\ dt$
    - $\displaystyle dy=y'(t) \to \int_Cf(x,y)dy=\int^b_af\big(x(t),y(t)\big).y'(t)\ dt$
    - $\displaystyle \int_{-C}f(x,y)dx=-\int_Cf(x,y)dx$

![Screenshot 2023-05-23 at 14.07.06.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/8185d94b-e43f-4c68-8dc8-4128baa257f7/Screenshot_2023-05-23_at_14.07.06.png)

- ***Line integrals in space: $\color{tomato}\displaystyle \int_C \bold F\cdotp d\bold r$
    
    - $\displaystyle {\color{tomato}\int_C f(x,y,z)ds} =\int^b_a f\big(x(t),y(t),z(t)\big).\sqrt{
    
    \bigg( \frac{dx}{dt}\bigg)^2+ \bigg( \frac{dy}{dt}\bigg)^2 + \bigg( \frac{dz}{dt}\bigg)^2 }
    
    dt\\ \color{tomato}=\int^b_a f\big(\bold r(t)\big) \ |\bold r'(t)| dt$
    
    - Line integral with respect to $z$:
        - $\color{tomato}\displaystyle dz=z'(t) \to \int_Cf(x,y,z)dz=\int^b_af\big(x(t),y(t),z(t)\big).z'(t)\ dt$
- ***Line integrals of vector fields:
    
    - Work done on moving an object on a curve in 3D space in a vector field (force/electric) is:
        - $\displaystyle {\color {tomato}W}=\int_C \bold F.d\bold r=\int_C \bold F\cdot \bold T\ ds \color {tomato}= \int^b_a \bold F\big( \bold r(t)\big) \cdotp \bold r'(t) \ dt$ (dot)
            - where $\displaystyle \bold T (x,y,z)=\frac{\bold r'(t)}{|\bold r'(t)|}$ is unit tangent vector
            - $\bold F(\bold r(t))$ means $\bold F(x(t),y(t),z(t))$

![Screenshot 2023-06-05 at 13.57.50.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/37b998db-234f-4e20-b328-8122ad625d0d/Screenshot_2023-06-05_at_13.57.50.png)

## The fundamental theorem for line integrals:

- Net change theorem for line integral:
    - Let $C$ be smooth curve by vector function $\bold r(t)$ and gradient vector $\Delta f$ continuous on $C$.
        - Then $\displaystyle\color{tomato} \int_C\Delta f\cdotp d\bold r = f\big(\bold r(b)\big)-f(\bold r(a)\big)$, true for 2 and 3 variables

![Screenshot 2023-06-05 at 20.28.24.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/0dead3fc-659e-48d6-af87-75f98fb71409/Screenshot_2023-06-05_at_20.28.24.png)

- Independence of path:
    - Line integrals of conservative vector fields are independent of path, $\displaystyle \int_{C_1} F\cdotp d\bold r= \int_{C_2} F\cdotp d\bold r$ if $C_1$ and $C_2$ have the same initial and terminal points
    - Closed curve: $\bold r_1(a)=\bold r_2(b)$ have $\int_C F\cdotp d\bold r=0$

![Screenshot 2023-06-05 at 20.42.37.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/970dcf37-e93d-4a3c-9977-52fa2624655f/Screenshot_2023-06-05_at_20.42.37.png)

$\int_{C_1} F\cdotp d\bold r=-\int_{-C_2} F\cdotp d\bold r$

- If $\bold F(x,y)=P(x,y)\bold i+Q(x,y)\bold j$ is a conservative vector field, where $P$ and $Q$ have continuous first-order $\partial$ then though out $D$ we have $\displaystyle \frac{\partial P}{\partial y}=\frac{\partial Q}{\partial x}$
- Let $\bold F(x,y)=P\bold i+Q\bold j$ be a vector field on an open simple-connected region $D$. Suppose $P$ and $Q$ have continuous first-order $\partial$ and $\displaystyle \frac{\partial P}{\partial y}=\frac{\partial Q}{\partial x}$ though out $D$ then $\bold F$ is conservative
- To test for conservative:
    - $\displaystyle \bold F=\Delta f=< \underbrace{\frac{\partial f}{\partial x}}_{M}, \underbrace{\frac{\partial f}{\partial y}}_{P}, \underbrace{\frac{\partial f}{\partial z}}_{Q}>$
    - Take pairs and test if $\frac{\partial M}{\partial y}=\frac{\partial P}{\partial x}, \frac{\partial M}{\partial z}=\frac{\partial Q}{\partial x}, \frac{\partial P}{\partial z}=\frac{\partial Q}{\partial y}$

![Screenshot 2023-06-05 at 20.55.30.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/c5b51343-04b6-43f6-a6e0-158ffda42629/Screenshot_2023-06-05_at_20.55.30.png)

![Screenshot 2023-06-05 at 20.58.29.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/0b0549a9-3b25-4190-b21d-6657321b179c/Screenshot_2023-06-05_at_20.58.29.png)

- Find potential function:
    - Integrate $f_x(x,y,z)$ with respect to $x$ to have ${\color{coral}f(x,y,z)}=\int f_x(x,y,z)dx + g(y,z)$
        - $g(y,z)$ as arbitrary constant of integration
    - Compare $f_y(x,y,z)$ with $y$ partial derive of found ${\color{coral}f(x,y,z)}$ to have $g_y(y,z)$
    - Integrate $g_y(y,z)$ with respeect to $y$ to have $\int g_y(y,z)dy+ h(z)$
        - $h(z)$ as arbitraty constant
    - Differentiate found $f$ with respect to $z$ to compare with $f_z$
- Conservation of energy:
    - Work done by the force field along $C$ is equal to the change in kinetic energy at the endpoints of $C$, $W=K(B)-K(A)$

## Green’s theorem: (2d version of stoke)

- Relates a double integral over a plane region $D$ to a line integral around its plane boundary curve.
- Positive orientation refers to counter clockwise traversal of $C$
- Let $C$ be a positively oriented, piecewise-smooth, simple closed curve in the plane. If $P (\bold Fi)$ and $Q$ have continuous partial derivatives on an open region that contains $D$
    - $\displaystyle\color{tomato} \oint_C \bold F \cdotp d\bold r= \oint_C P\ dx + Q\ dy=\int\int_D\bigg( \frac{\partial Q}{\partial x}-\frac{\partial P}{\partial y} \bigg)dA$
        - If $P(x,y)=Q(x,y)=0\to\oint_C P\ dx + Q\ dy=0$
    - The curl along the line equals to total curl on the graph because inside, curls cancels out
    - Green’s theorem also work with regions with holes

![Screenshot 2023-06-06 at 06.57.39.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/9382a287-8652-46d0-94f0-e218134676c7/Screenshot_2023-06-06_at_06.57.39.png)

![Screenshot 2023-06-06 at 07.30.35.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/b0397b04-dde0-4fde-84eb-3938d0daa2ac/Screenshot_2023-06-06_at_07.30.35.png)

- Since the area of $D= A= \int\int _D1 \ dA$, we choose $\frac{\partial Q}{\partial x}-\frac{\partial P}{\partial y}=1$, then:
    - $\displaystyle A=\oint_C x\ dy=-\oint _C y\ dx=\frac12 \oint_C x\ dy-y\ dx$

## Curl and divergence:

- Curl: $\text {curl } \bold F\color{tomato}= \nabla \times \bold F$
    - $\bold F={\color{tomato}P} \ \bold i + {\color{tomato}Q} \ \bold j + {\color{tomato}R}\ \bold k$, a vector field and the partial derivatives all exist
        
        - $\displaystyle \text {curl } \bold F=
        
        \bigg( \frac{\partial R}{\partial y}-\frac{\partial Q}{\partial z} \bigg)\bold i+ \bigg( \frac{\partial P}{\partial z}-\frac{\partial R}{\partial x} \bigg)\bold j+ \bigg( \frac{\partial Q}{\partial x}-\frac{\partial P}{\partial y} \bigg)\bold k$
        
    - Vector, represents tendency to spin around an axis with magnitude measures the strength of the rotation and direction indicates the axis of rotation
        
    - If a function $f$ of 3 variables that has continuous second-order partial derivatives, then $\color{tomato}\text{curl }(\nabla f)=0$
        
        - Since $\bold F=\nabla f$ is conservative vector field, then if $\bold F$ is conservative then $\text{curl } \bold F=0$
        - $\text{curl } \bold F=0$ then $\bold F$ is conservative if $\bold F$ is simply connected

![Screenshot 2023-06-06 at 10.10.26.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/ba69e04f-ec91-42dc-bc0c-f7b99c6c7fd4/Screenshot_2023-06-06_at_10.10.26.png)

$\nabla=\{\frac{\partial}{\partial x},\frac{\partial}{\partial y},\frac{\partial}{\partial z}\}$ treated as a variable

- Divergent: $\color{tomato}\text {div } \bold F= \nabla \cdotp\bold F$
    - If $\bold F={\color{tomato}P} \ \bold i + {\color{tomato}Q} \ \bold j + {\color{tomato}R}\ \bold k$, a vector field and the partial derivatives of $P, Q$ and $R$ **all exist, then the **div** of $\bold F$ ****is the vector field on 3 defined by $\color{tomato}\text {curl } \bold F= \nabla \times \bold F$
        - $\displaystyle \text {div } \bold F= \frac{\partial P}{\partial x}+ \frac{\partial Q}{\partial y}+ \frac{\partial R}{\partial z}$
        - $\color{tomato}\text{div curl }\bold F=0$ always because $a\cdotp (a\times b)=0$, otherwise $\text{curl } \bold F$ doesnt exist
    - Scalar, represents tendency for fluid to diverge away from that point, $\text{div }\bold F=0$ is said to be incompressible

![Untitled](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/b785fbeb-36c1-409e-a5a0-8e6b0deb6504/Untitled.png)

- Vector form of Green’s theorem:
    - $\displaystyle{ \color{tomato} \oint_C \bold F \cdotp d\bold r }= \int\int _D(\text{curl } \bold F)\cdotp \bold k \ dA$
    - Second form of Green’s theorem:
        - $\displaystyle{ \color{tomato} \oint_C \bold F \cdotp \bold n \ ds}= \int\int _D\text{div } \bold F(x,y)\ dA$

![Screenshot 2023-06-10 at 16.21.26.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/313d0a67-6f28-41fb-abd5-9975288cae4f/Screenshot_2023-06-10_at_16.21.26.png)

## Parametric surface and their areas: (parameterised when possible)

- Parametric surfaces: $S$
    - $\bold r(u,v)=x(u,v)\ \bold i+y(u,v)\ \bold j+z(u,v)\ \bold k$ with parametric equations, $x=x(u,v)$
    - $\bold r(u_0,v)$ is a grid curve

![Screenshot 2023-06-12 at 13.50.45.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/72197c08-082f-481b-8c05-e07e482b9de3/Screenshot_2023-06-12_at_13.50.45.png)

- Convert from to cylindrical, polar, spherical coordinates
    
    - Vector function that contains vector $\bold a$ and $\bold b$, and pass through $\bold r_0(u,v)$ is $\bold r(u,v)=\bold r_0+u\bold a+v\bold b$
    
    ![Screenshot 2023-06-12 at 21.50.34.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/9fde3df8-df10-4f40-9278-cf3ba4d1ed13/Screenshot_2023-06-12_at_21.50.34.png)
    
    - From the spherical coors:$\\ \bold r(u,v)={\color{tomato}a\sin\phi\cos\theta }\ \bold i+ {\color{tomato}b\sin\phi\sin\theta}\ \bold j + {\color{tomato}c\cos\phi}\ \bold k$
    
    ![Screenshot 2023-06-12 at 22.20.38.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/98043b1d-34b9-4234-835d-dcccac16c623/Screenshot_2023-06-12_at_22.20.38.png)
    
- Surface of revolution:
    
    - Surface $S$ obtained by rotating the curve $y=f(x)$ about the $x$-axis is:
        - $x=x, y={\color{tomato}f(x)}\cos\theta, z={\color{tomato}f(x)}\sin\theta$ where $u=x,v=\theta$
    - Convert to parametric equations by simplifying the equations when 2 of xyz variables can be replaces

![Screenshot 2023-06-12 at 15.11.59.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/84dcd175-cd6b-4c62-83d8-241c08657a31/Screenshot_2023-06-12_at_15.11.59.png)

- Tangent plane:
    - $\displaystyle \bold r_u=\frac{\partial x}{\partial u}(u_0,v_0)\bold i+\frac{\partial y}{\partial u}(u_0,v_0)\bold j+\frac{\partial z}{\partial u}(u_0,v_0)\bold k$
    - so normal of tangent plane, $\bold r_n=\bold r_u\times\bold r_v$
        - 0 if it has corner

![Screenshot 2023-06-12 at 14.49.05.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/24752fce-8dc4-4b30-a081-1084dcb08fee/Screenshot_2023-06-12_at_14.49.05.png)

- Surface area:
    - $\displaystyle A(S)=\int\int_D{\color{tomato} |\bold r_u\times \bold r_v|}dA$

![Screenshot 2023-06-12 at 16.33.53.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/caaa9dc4-0a70-4402-9d1f-697c5228b31d/Screenshot_2023-06-12_at_16.33.53.png)

- Surface area of the graph of a function:
    
    - For surface $S$ with equation $x=x,y=y, \color{tomato}z=f(x,y)$
    - $\displaystyle \bold r_x= \bold i +\bigg(\frac{\partial f}{\partial x}\bigg)\bold k$ and $\displaystyle \bold r_y= \bold j +\bigg(\frac{\partial f}{\partial y}\bigg)\bold k$
    - $\displaystyle A(S)=\int\int_D {\color{tomato}\sqrt{1 + \bigg( \frac{\partial z}{\partial x}\bigg)^2
    
    +\bigg( \frac{\partial z}{\partial y}\bigg)^2}}dA$
    

![Screenshot 2023-06-12 at 16.36.58.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/f02d186e-aeb8-4b18-8dd5-c6c877864c17/Screenshot_2023-06-12_at_16.36.58.png)

## Surface integrals:

- Parametric surfaces:
    - $\displaystyle\int\int_S f(x,y,z)\ dS=\int\int_D {\color{tomato} f\big(\bold r(u,v)\big) .|\bold r_u \times \bold r_v|\ }dA$

![Screenshot 2023-06-12 at 16.50.23.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/8669877c-b43c-4649-9721-0789873d0c08/Screenshot_2023-06-12_at_16.50.23.png)

- Graph: for surface $S$ with equation $x=x,y=y, \color{tomato}z=g(x,y)$
    
    - $\displaystyle\int\int_S f(x,y,z)\ dS=\int\int_D {\color{tomato} f\big(z,y,g(x,y)\big) \sqrt{ 1+\bigg( \frac{\partial z}{\partial x} \bigg)^2+
    
    \bigg( \frac{\partial z}{\partial y} \bigg)^2} \ }dA$
    
    - use $x=g(y,z)$ or $y=g(x,z)$ if necessary

![Screenshot 2023-06-12 at 17.09.09.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/aaa8b023-7654-4fda-9abf-e21882b6acfa/Screenshot_2023-06-12_at_17.09.09.png)

- Oriented surface:
    
    - There are two possible orientations for any orientable surface
        
    - Positive orientation: normals point outward, concave inward
        
    
    ![Screenshot 2023-06-16 at 01.32.00.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/341720fd-fe43-41d8-a261-4f4c40fe815e/Screenshot_2023-06-16_at_01.32.00.png)
    

Mobius strip

![Screenshot 2023-06-16 at 01.28.37.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/36e57357-7605-4929-a468-9533cd4caa4e/Screenshot_2023-06-16_at_01.28.37.png)

### Surface integral of vector fields:

- $\bold F$ is a continuous vector field on oriented surface $S$ with uni normal vector $\bold n$, then surface integral of $\bold F$ over $S$ (known as the flux of $\bold F$ across $S$) is
    
    - $\displaystyle \int\int\limits_S {\color{tomato}\bold F\cdotp dS}=\int\int\limits_S {\color{tomato}\bold F\cdotp \bold n\ dS}
    
    =\int\int\limits_D \color{tomato}\bold F\cdotp (\bold r_u\times \bold r_v) \ dA$
    
    - If surface $S$ is given by graph $z=g(x,y)$ then change to xy and:
        
        - $\displaystyle \int\int\limits_S {\color{tomato}\bold F\cdotp dS}=\int\int\limits_D
        
        {\color{tomato}\bigg(-P\frac{\partial g}{\partial x}-Q\frac{\partial g}{\partial y} + R\bigg)} \ dA$
        

![Screenshot 2023-06-16 at 01.47.25.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/34534a04-d376-4ece-9670-5571b57825d9/Screenshot_2023-06-16_at_01.47.25.png)

*$P QR$ is from $\bold F$

- There might be 2 or more parts in a closed surface
- Electric flux of electric field $\bold E$ though surface $S$: $\displaystyle \int\int\limits _S \bold E\cdotp dS$
- The net rate of outflow of substance through outward oriented surface $S$: $\displaystyle\int\int\limits_S \bold F\cdotp dS$
    - where $\bold F=p(\bold x)\bold v(\bold x)$, density times velocity
- Temperate of any point is $u(x,y,z)$ the heat flow is defined as a vector field: $\bold F=-K\nabla u$
    - then the rate of heat flow across surface $S$ is $\displaystyle\int\int\limits_S \bold F\cdotp dS=-K\int\int \nabla u \cdotp dS$

## Stoke’s theorem: (3d version of green)

- Relates a surface integral over a surface $S$ to a line integral around the boundary space curve of $S$
    
- The orientation of surface $S$ is the positive orientation of boundary curve $C$
    
- Let $S$ be an oriented piece-wise smooth surface that is bounded by a simple, closed, piecewise-smooth boundary curve $C$ with positive orientation
    
    - $\displaystyle\color{tomato} \oint_C \bold F \cdotp d\bold r\equiv
    
    \int\int_S \text{curl }\bold F\cdotp dS$, curl $\bold F$ is treated as vector field
    
- If the surface $S$ is a graph function, $z=g(x,y): \displaystyle
    

\int\int_S \text{curl }\bold F\cdotp dS$

```
![Screenshot 2023-06-17 at 00.36.06.png](<https://s3-us-west-2.amazonaws.com/secure.notion-static.com/459fa1da-377f-4829-8af9-fbe55af5e0ea/Screenshot_2023-06-17_at_00.36.06.png>)
```

![Screenshot 2023-06-16 at 23.58.47.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/4b83e2f7-5cc6-48be-9cc6-76df873850be/Screenshot_2023-06-16_at_23.58.47.png)

![Screenshot 2023-06-16 at 23.16.13.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/b885d31b-91f3-41d7-976d-5b21184b0228/Screenshot_2023-06-16_at_23.16.13.png)

![Screenshot 2023-06-17 at 00.33.20.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/e9c1cb10-339b-4cb3-b15d-7925768ca1bd/Screenshot_2023-06-17_at_00.33.20.png)

- If $S_1$ and $S_2$ are oriented surfaces with same oriented boundary curve $C$ and both satisfy the hypotheses of Stoke’s theorem: $\displaystyle \int\int_{S_1} \text{curl }\bold F\cdotp dS= \int_C\bold F\cdotp d\bold r =\int\int_{S_1} \text{curl }\bold F\cdotp dS$, Both curl F integral are equal

![Screenshot 2023-06-22 at 14.03.38.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/90aa3c34-6bcd-4f00-abb5-6ae2dd99ea0f/Screenshot_2023-06-22_at_14.03.38.png)

## The divergence theorem:

- 3D vector version of green theorem: $\int_C \bold F\cdotp \bold n \ ds$:
    
    - Let $E$ be a simple solid region, $S$ be the boundary surface of $E$, given with positive (outward) orientation. $\bold F$ is vector field whose component functions have continuous partial derivatives on an open region that contains $E$. Then:
        - $\displaystyle\int\int _S\bold F\cdotp dS=\int\int_S\color{tomato} \bold F\cdot \bold n\ dS = \int\int\int_E \text{div } \bold F\ dV$, use triple integral
- A region $E$ is inside $S_2$ but outside $S_1$:
    
    - $\displaystyle\int\int_S\text{div } \bold F\ dV =\color{tomato}-\int\int_{S_1}\bold F\cdotp dS+\int\int_{S_2}\bold F\cdotp dS$

![Screenshot 2023-06-22 at 16.21.48.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/4fa6de42-67b4-460e-9dbf-023469985e9a/Screenshot_2023-06-22_at_16.21.48.png)

---