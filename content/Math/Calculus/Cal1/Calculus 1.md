---
Credits: 4
Done: true
tags:
  - Math/calculus
---
$$ \text{Chapter 1: Functions and limits} $$

## 1.1: Functions and limits

- Function
    - independent vs dependent
- Qualitative & quantitative data (continuous, discrete)
- Function presentation:
    - cartesian graph
    - formula
    - descriptive
    - table
- Vertical line test: no value of domain has 2 values in range
- Piecewise defined function: different formulae for different parts of the domain
- Symmetric property: put $-x$ as input to check
    - even: $f(-x)=f(x)$
    - odd: $f(-x)=-f(x)$
- Increasing vs decreasing function

## 1.2: A catalog of essential functions

- Mathematical model is a mathematical description of a real-world phenomenon
    
    - linear function: $y=mx+c$
    - polynomial function: $y=ax^3+bx^2+cx+d$
        - the one-term function’s degree of the polynomial dictates if the graph is odd or even
    - power function:
        - type 1: $y=x^a$
        - type 2: $y=x^{1/n}$, $n^{th}$ roots of $x$
        - reciprocal: $y=x^{-1}$
    - rational function: ratio of 2 polynomial, $f(x)=P(x)/Q(x)$
- Transformation of functions:
    
    - Vertical and horizontal shifts
    - Vertical and horizontal stretching, shrinking and reflecting
- Combinations of functions: plus minus divide multiply, $(f+g)(x)=f(x)\pm g(x)$
    
    - Domains of the new function is $f\land g$, because both functions have to be defined
- Composite function : $(f\circ g)(x)=f(g(x))$
    

## 1.3: The limit of a function:

- $\lim\limits_{x\to a}f(x)=L$, limit of $f(x)$ as $x$ approaches $a$ equals to $L$, but not a
    - if $x=a$ is not defined, draw a table to check the closest value $x=a\pm 0.01$ thus assuming the limit of a function for an undefined constant
- One-sided limit:
    - $\lim\limits_{x\to a^+}f(x)=L$ means $x$ approaches $a$ from the right side, $a^-$ means from the left
    - if $\lim\limits_{x\to a^-}f(x)\not=\lim\limits_{x\to a^+}f(x)$ then the curve has discontinuity and limit doesn’t exist

## 1.4: Calculating limits:

- Limit laws: only if both exists and finite

![Screenshot 2022-10-13 at 09.32.55.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/f1022dc5-9c1c-42e3-812c-f565bc1d0a9d/Screenshot_2022-10-13_at_09.32.55.png)

- Special trig limits:
    - $\lim\limits_{\theta \to 0}\frac{\cos\theta -1}{\theta} =0$
    - $\color{tomato}\lim\limits_{\theta \to 0}\frac{\sin\theta}{\theta} =1$, convert to this

![Screenshot 2022-10-13 at 09.34.17.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/26c9f379-4571-4264-ab67-b17d865d1164/Screenshot_2022-10-13_at_09.34.17.png)

- Split big term into a lot of smaller terms with the same limit approaching same x

## 1.5: Continuity:

- A function $f(x)$ is continuous if and only if:
    - $f(a)$ is defined
    - $\lim\limits_{x\to a}f(x)$ exist, both from the left and right
    - $\lim\limits_{x\to a}f(x)=f(a)$
- Removable discontinuity: only one value of the graph can be written in piecewise
- Infinite discontinuity: limit tends to infinity. Jump discontinuity: stair form of graph
- Polynomials, rational, functions, trigonometric functions are always continuous
- The intermediate value theorem: in a closed interval of $a<x<b$, the line cant jump thru $f(a)$ and $f(b)$ so $f(c)=0$f if $a<c<b$
- Squeeze theorem:
    - If $f(x)\le gx\le h(x)$ when $x$ is near a and $\lim\limits_{x\to a}f(x)=\lim\limits_{x\to a}h(x)=L$
    - Then $\lim\limits_{x\to a}g(x)=L$

## 1.6: Limits involving infinity:

- Infinite limit at $a$ makes a vertical asymptote at $x=a$
- Horizontal asymptote: when a close enough constant will tends the increase of $f(x)$ to another constant
- if $P(x)$ and $Q(x)$ are functions of $x^n$:
    - $\lim\limits_{x\to \infin}\frac{P(x)}{Q(x)}=\lim\limits\frac{\text{leading term of P}}{\text{leading term of Q}}$ bcz the biggest term would dominate

$$ \text{Chapter 2: Derivative} $$

## 2.1: Derivative and rate of change:

- Tangent problem, limit definition
    
- Instantaneous rate of change, $f'(a)=m=\lim\limits_{x\to a}\frac{f(x)-f(a)}{x-a}={\color{tomato}\lim\limits_{h\to 0}\frac{f(a+h)-f(a)}{h}}=\lim\limits_{\varDelta x\to 0}\frac{\varDelta y}{\varDelta x}$
    
    - first principle, second principle
    
    ![Screenshot 2022-10-14 at 00.10.07.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/26a663ce-c264-4f09-b771-c6cf0f79397d/Screenshot_2022-10-14_at_00.10.07.png)
    

## 2.2: The derivative as a function:

- If $f(x)$ is differentiable at $a$, then $f(x)$ is continuous at $a$
    
    - Not necessarily differentiable if $f(x)$ is continuous
- The derivative of a function might not exist if at $a$, it’s:
    

![Screenshot 2022-10-14 at 00.10.39.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/2ab90a5f-223d-43a2-b8ae-fdc137c46499/Screenshot_2022-10-14_at_00.10.39.png)

## 2.3: Basic differentiation formulas:

- $\frac d{dx}(x^n)=nx^{n-1}$ for $n$ of any real number
- Derivative rules: Product rule, Sum & difference rule
- $Sinx\xrightarrow[dx]{1} Cosx\xrightarrow[dx]{1}-Sinx\xrightarrow[dx]{1}-Cosx\xrightarrow[dx]{1}Sinx$

## 2.4: The product and quotient rule:

- Product rule, $(fg)'=fg'+gf'$
- Quotient rule, $(\frac f g)'=\frac{gf'-fg'}{g^2}$
- Trigonometry functions:
    - Find $\frac d{dx}Tan(x),\frac d {dx}Csc (x),\frac d{dx}Sec(x), \frac d{dx} Cot(x)$ by quotient rule

## 2.5: The chain rule, power rule combined with the chain rule:

## 2.6: Implicit differentiation:

- Differentiate both $x$ and $y$ at the same time, $\frac d{dx}y=\frac{dy}{dx}$

## 2.7: Related rate of change:

- Connected rate of change

## 2.8: Linear approximations and differentials:

- $L(x)\approx \color{tomato}f(x)=f(a)+f'(a).(x-a)$ bcz $=f(a)-f'(a).a+f'(a).x$
- $dy=f'(x).dx$ and $dx$ can be an independent variable and take a constant

### Extra:

- Marginal cost: cost of making a new product given x product is already produced
    - Total cost of x products: $f(x)$ then marginal cost
- Logistic function: infinitively increasing or decreasing
    - Derivative of logistic function is called surge function, rise quickly then level down

$$ \text{Chapter 3: Inverse Functions} $$

## 3.1: Exponential functions:

- Laws of exponential
- Natural exponential, $\color{tomato}e=\lim\limits_{x\to 0}(1+x)^{1/x}$

## 3.2: Inverse functions and logarithms:

- One-to-one function, where 1 value of x has 1 value of y and vice versa
    
    - No horizontal line intersect the graph more than once, thus invertible
    - If vertical line intersects the graph more than once then it’s not a function
- The domain of f(x) becomes range of its inverse and vice versa
    
- The graph of $f^{-1}x$ is reflection of $fx$ over the line $y=x$
    
- For inverted function:
    
    $f(y)=x\implies f'y.\frac{dy}{dx}=1\implies f'y=\frac{1}{dy/dx}$
    
    - Gradient at point $(a,f^{-1}a)$ on $f^{-1}x$ is equal to reciprocal of $f'x$ at $(f^{-1}a,a)$
    - $(f^{-1})'a=\frac{1}{f'(f^{-1}a)}$

![91702FA9-5FD2-443B-8CAD-4CBD98F2D856.jpeg](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/9817f9a7-03be-47ce-889f-ce4b4695cfd3/91702FA9-5FD2-443B-8CAD-4CBD98F2D856.jpeg)

- Laws of logarithms
- $\log_ax=\frac{\ln x}{\ln a}$

## 3.3: Derivatives of logarithmic and exponential functions:

- $f(x)=\log_ax=\frac{\ln x}{\ln a}\implies f'(x)=\frac 1x\log_a e=\frac 1{x.\ln a}$
- $\frac d {dx}(\ln x)=\frac 1 {x}$
- Logarithmic differentiation:
    - Take natural log both sides and use laws of log to simplify
    - Differentiate implicitly
    - Make dy/dx the subject
- $f(x)=a^x\implies \color{tomato}\frac d{dx}(a^x)=a^x\ln a$
- Using logarithmic differentiation: take log before differentiating

## 3.4: Exponential growth and decay:

- Law of natural growth and decay, $\frac{dy}{dt}=ky$, rate of change is proportional to its size
    - Solution is in the form: $y=C.e^{kt}$
- Radioactive decay, $\frac{dm}{dt}=-km$, rate of decay is proportional to its mass
    - Solution is in the form, $m=m_o.e^{-kt}$
- Decreasing, losing, leaking, cooling down,.. means the rate of change is negative
- First order differential equation
- Newton’s law of cooling: rate of cooling an is proportional to the temperature difference between the object and its surroundings
    - $\frac{dT}{dt}=k(T-T_0)$ then solution is $f(t)=y_0e^{kt}$

## 3.5: Inverse trigonometric functions:

- Differentiate implicitly for inverse trig
    
- $\cos^2x+\sin^2x=1$
    
- $\color{tomato}\sec^2x=1+\tan^2x$
    
- $\csc^2x=\cot^2x+1$
    
- $\frac d {dx}(\sin ^{-1}(x))=\frac 1 {\sqrt{1-x^2}}$
    
    - $-\frac \pi2\le x\le \frac \pi2$ and $-1\le f(x)\le 1$
- $\frac d {dx}(\cos ^{-1}(x))=-\frac 1 {\sqrt{1-x^2}}$
    
    - $0\le x\le \pi$ and $-1\le f(x)\le 1$
- $\frac d {dx}(\tan ^{-1}(x))=-\frac 1 {{1+x^2}}$
    
    - $-\pi/2\le x\le \pi/2$ and $-\infin\le f(x)\le \infin$

## 3.6: Hyperbolic functions:

- $\sinh(x)=\frac{e^x-e^{-x}}{2}$
- $\cosh(x)=\frac{e^x+e^{-x}}{2}$
- Inverse hyperbolic functions

![Screenshot 2022-10-15 at 18.03.47.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/1b5226fe-a8bb-4f57-bda9-5c289bdb5f8e/Screenshot_2022-10-15_at_18.03.47.png)

![Screenshot 2022-10-15 at 17.57.19.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/a7f6e739-edf9-4cc1-9227-7f69cf7d7aec/Screenshot_2022-10-15_at_17.57.19.png)

![Screenshot 2022-10-15 at 17.57.45.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/9c327ef8-740a-42c8-839c-6c8c2072ece2/Screenshot_2022-10-15_at_17.57.45.png)

![Screenshot 2022-10-15 at 18.01.58.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/31631def-e405-4baf-95a0-40b3d8e2b0df/Screenshot_2022-10-15_at_18.01.58.png)

## 3.7: Indeterminate forms and l’hospital’s rule:

- Form of type $\frac 0 0$ and $\frac \infin \infin$ where quotient of 2 functions have same limit makes it indeterminable
    
- Form of type $0\times \pm \infin$ where $\lim\limits_{x\to a}f(x).g(x)$ as $\lim\limits_{x\to a}f(x)=0$ and $\lim\limits_{x\to a}g(x)=\pm \infin$
    
    - Convert the multiplication to $\lim\limits_{x\to a}\frac{f(x)}{g(x)}$ to solve by l’hospital’s rule
- Form of type $\infin - \infin$ where $\lim\limits_{x\to a}[f(x)-g(x)]$ as $\lim\limits_{x\to a}f(x)=\infin$ and $\lim\limits_{x\to a}f(x)=\infin$
    
    - Convert the difference to one fraction with common denominator
- Forms of powers types: ($\lim\limits_{x\to a}[f(x)]^{g(x)})$
    
    - $0^0$ where $\lim\limits_{x\to a}f(x) = 0$ and $\lim\limits_{x\to a}g(x) = 0$
    - $\infin^0$ where $\lim\limits_{x\to a}f(x) = \infin$ and $\lim\limits_{x\to a}g(x) = 0$
    - $1^\infin$ where $\lim\limits_{x\to a}f(x) = 1$ and $\lim\limits_{x\to a}g(x) = \pm\infin$
    
    $\implies$ $\ln y=\ln f(x)^{g(x)}=g(x).\ln|f(x)|$ or write $f(x)=e^{\ln(f(x)}$
    
    $\implies$ then find $\lim\limits_{x\to a} \ln y$ then find $y=e^{\ln y}$
    
- l’Hospital’s rule, a systematic method, for evaluating only indeterminate forms
    
    - $\lim\limits_{x\to a}\frac{f(x)}{g(x)}=\lim\limits_{x\to a}\frac{f'(x)}{g'(x)}$
    - Also true for $x\to a^+, a^-, \infin,-\infin$ and one-sided limits
- Use l’hospital’s rule 2 times if the result of the first time applied is still indeterminable
    

$$ \text{Chapter 4: Applications of differentiation} $$

## 4.1: Max and min values:

- Extreme values are absolute max and min values or endpoints(if included)
    - They could be one of the critical number or one of the end points
- Local maximum and local minimum value are bigger than others value near it
    - $a$ is a local max or min if $f'(a)=0$, by Fermat’s theorem
- Extreme value theorem: If $f$is continuous on a closed interval $[a,b]$ then $c$ and $d$ are min and max somewhere in the middle of $[a,b]$
- Fermat’s theorem: if $f$ has local min or max at $c$ and if $f'(c)$ exist then $f'(c)=0$
- Critical number of function $f(a)$ are numbers that $\color{tomato}f'(a)=0$ or $f'(a)$ doesn’t exist
    - If $f$ has local min or max at $c$, then $c$ is a critical point of $f$
    - End points has has no $f'(a)$, thus they are critical numbers

## 4.2: The mean value theorem:

- By Rolle’s theorem, if:
    
    - $f$ is continuous on the closed interval $[a,b]$
    - $f$ is differentiable on on interval $(a,b)$
    - $f(a)=f(b)$
    
    $\implies$ then there is a number in the interval $(a,b)$ such $f'(c)=0$
    

![Screenshot 2022-10-15 at 22.18.43.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/fc6c94c6-d886-4a46-af3d-2fd9ff112632/Screenshot_2022-10-15_at_22.18.43.png)

- Prove that the equation has only 1 root:
    
    - Given the equation is continuous, find $a$ and $b$ where $f(a)<0$ and $f(b)>0$
        - Thus, $a< \text{root}<b$
    - Show that $f'(x)\not =0$ or $f'(x)<>0$ for all $x$ so the curve never head back down again
- By the mean value theorem, if:
    
    - $f$ is continuous on the closed interval $[a,b]$
    - $f$ is differentiable on on interval $(a,b)$
    
    $\implies$then a number in the interval $(a,b)$ such $\color{tomato}f(b)-f(a)= f'(c)(b-a)$, same gradient
    

![Screenshot 2022-10-15 at 22.17.47.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/d77c8205-6b2b-4e55-919d-022bb07ad457/Screenshot_2022-10-15_at_22.17.47.png)

## 4.3: Derivatives and the shapes of graphs:

- Increasing/decreasing test
    
- if $f'(x)$ of one interval (boundaries are critical points)’s sign is known , we can’t assume the 2 neighbour intervals’ signs because of inflexion point
    
- if $f'(x)$ change from negative to positive then it’s local minimum point and same for maximum
    
- Second derivative, $f''(x)$: concavity
    
    - $f''(x)=0$ at inflection point, the point on a continuous curve where the graph change its concavity from CU to CD or vice versa
        - only when $f'(x)$ change signs, from negative to positive or vice versa
            - meaning the graph of $f''x$ cross x-axis
    - $\color{tomato}f''(x)>0$ then the curve concave upward
    - $\color{tomato}f''(x)<0$ then the curve concave downward

![Screenshot 2022-10-16 at 14.48.06.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/ea118c52-abe7-4904-b3ce-db223bcc44ba/Screenshot_2022-10-16_at_14.48.06.png)

![Screenshot 2022-10-16 at 14.51.08.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/7c6bf9ef-e5a0-4f64-a610-c92d61dad2ea/Screenshot_2022-10-16_at_14.51.08.png)

- Draw graph by including:
    - $f'(x)$ with critical points $f'(x)=0$ and its intervals
    - $f''(x)$ with critical points $f''(x)=0$ and its intervals

## 4.4: Curve sketching:

- Domain
- Intercepts
- Symmetry, periodic
- Asymptotes, limits
- Interval of increase and decrease
- Local max and min points
- Concavity and points of inflection, includes all intervals of both differentiations
- Sketch, good luck

## 4.5: Optimisation problems:

- Form 1 big equation then differentiate implicitly
- In business and economics:
    - $R(x)=x.p(x)$ where $R(x)$ is revenue function and $P(x)$ is price function, x is the nb of products
    - Function of profit, $P(x)=R(x)-C(x)$ where $C(x)$ is cost function

## 4.6: Newton’s method:

- To find the roots of polynomials of degrees $>4$, using linear approximation
- The root $=\lim\limits_{n\to \infin}x_n$$=\lim\limits_{m\to \infin}x_n$$=\lim\limits_{x\to \infin}x_n$

$\displaystyle \color{tomato}x_{n+1}=x_n-\frac{f(x_n)}{f'(x_n)}$

$$ \text{Chapter 5: Integrals} $$

## 5.1: Areas and distances:

- Area under graph by the sum of the areas of approximating rectangles:
    - Principle is as same as limits of area, the $f(x)$ value can be:
        - Left end point of the rectangle
        - Right end point of the rectangle
        - Take $f(x)$ as the midpoint of 2 of its endpoints, called sample points $x^*_n$
            - $x^*_n=\frac{x_{n}+x_{n+1}}{2}$, not mid-value ($\not= \frac{f(x_1)+f(x_2)}2$)

## 5.2: The definite integral:

- By Riemann sum, $f(x)$ is defined on $[a,b]$, then : $A\approx\lim\limits_{n\to \infin}\sum\limits^n_{i=1}f(x_i^*)\Delta x$
    
    - where $\Delta x_i$ is separate subinterval length for each subinterval, need not to be equal
    - sample point, $x_i^*$ can be anywhere on the $i^{th}$ subinterval, need not to be mid point
    - If the limit exist then $A=\int^b_a f(x)dx$
- Net change theorem: $\int^b_a \frac{dfx}{dx}dx=f(b)-f(a)$
    
    - The integral of rate of change of a function equals to the net change in the function
    - If the area has both positive and negative values then the integral gives net area
- $\sum\limits^n_{i=1}i=\frac{n(n+1)}{2}$
    
- $\color{tomato}\sum\limits^n_{i=1}i^2=\frac{n(n+1)(2n+1)}{6}$
    
- $\color{tomato}\sum\limits^n_{i=1}i^3=[\frac{n(n+1)}{2}]^2$
    
- Definition of integral: If $f$ is integrable on $[a,b]$ then
    
    - $\int^b_a f(x)dx=\lim\limits_{n\to \infin} \sum f(x_i).\Delta x$ where $\color{tomato}x_i=a+i.\Delta x$
- Midpoint rule: the midpoint of each rectangle is used to compute
    
    - $\int^b_af(x)dx\approx\sum\limits^n_{i=1}f(\bar x).\Delta x$ where $\bar x=\frac 12(x_{i-1}+x_i)$
- Properties of the integrals: the area under graph is smaller than the large rectangle and bigger than the smaller rectangle
    
    - If $m\le f(x)\le M$ for $a\le x\le b$:
        
        $\implies m(b-a)\le \int^b_a f(x)dx\le M(b-a)$
        

## 5.3: Evaluate definite integrals:

- Evaluation theorem:
    - $\int^b_af(x)dx=F(b)-F(a)$ where $F'(x)=f(x)$
- Definite integral (without limits) results to a constant number
- Indefinite integral (without limits) is a function and requires to add C, arbitrary constant

![Screenshot 2022-10-17 at 12.20.28.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/066594bd-3d16-45c8-93b6-081a7a791133/Screenshot_2022-10-17_at_12.20.28.png)

$\int a^xdx \text{***}$

## 5.4: The fundamental theorem of calculus:

- If $f$ is continuous and $g(x)=\int^x _a f(t) dt$ then $g(x)$ is a function of area under graph $f$
- The mean value theorem for integrals:
    - If $f$ is continuous on $[a,b]$ then there is a number, mean value, between a and b where $f(c)=\frac 1{ b-a}\int^b_af(x)dx$
        - So mean value = area/domain

## 5.4: The substitution rule:

- $\int f[g(x)]g'(x)dx=\int f(u)du$ where $u=g(x)$ then use $g'(x)$ to cancel out term in $f(x)$
    - Where the limits in terms of $x$ is changed to limits in term of $u$

$$ \text{Chapter 6: Techniques of integration} $$

## 6.1: [[Integration by parts]]


## 6.2: Trigonometric integrals and substitution:

- Try to write an integrand involving powers of sine and cosine in a form where we have only one sine factor (and the remainder of the expression in terms of cosine) and vice versa
    
    - Then use $\cos^2(x)+\sin^2(x)=1$
- Half-angle formulae:
    
    - $\cos 2x=\color{tomato}1-2\sin^2x=2\cos^2x-1$
    - $\sin 2x=2\cos x\sin x$
- $\int \tan x dx=\ln|\sec x|+c$
    
- $\int \sec x dx=\ln|\sec x+\tan x|+c$
    

![Screenshot 2022-10-17 at 14.51.48.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/312a6885-9f6c-463b-a174-716aea33c246/Screenshot_2022-10-17_at_14.51.48.png)

- Integrate by substitution:
    
    - To transform difficult integral to simpler integral
    - The new integrand must be rewritten in terms of the new variable, u.
    - Either cancel out some terms of x when substitute u in or rewritten entire integrand in term of u
    - Convert limits of $x$ to limits in term of $u$ for definite integral
- Inverse substitution
    

![Screenshot 2022-10-18 at 18.52.10.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/5021837b-a29e-4a8c-8137-689163a441c2/Screenshot_2022-10-18_at_18.52.10.png)

## 6.3: Partial fractions:

- Case 1: $\frac{px+q}{(ax+b)(cx+d)}=\frac{A}{ax+b}+\frac B {cx+d}$
- Case 2: $\frac{px^2+qx+r}{(ax+b)^3x^2}=\frac{A}{(ax+b)^3}+\frac B {(ax+b)^2}+\frac{C}{ax+b}+\frac D {x^2}+\frac E{x}$
- Case 3: non factorisable $\frac{px^2+qx+r}{(ax-b)(cx^2+d)}=\frac A{ax-b}+\frac{Bx+C}{cx^2+d}$, one degree lower
- Case 4: repeat non factorizable ${\color{tomato}\frac{px^2+qx+r}{(ax-b)(cx^2+dx+e)^n}}=\frac{A}{ax-b}+\frac{Bx+C}{(cx^2+bx+e)^1}+.+\frac{Yx+Z}{(cx^2+bx+e)^n}$

## 6.5: Approximate integration:

- Types of area approximation:
    - Left-end points
    - Right-end points
    - Trapezoidal Rule
    - Mid-point
    - Simpson’s rule
- Trapezoidal rule: (trapezium rule)
    - $\int^b_af(x)dx=\frac{\Delta x}{2}[f(x_0)+2f(x_1)+2f(x_2)+...+f(x_n)]$
        - Use sum of y-values, different from Riemann’s sum
- Error bounds:
    - For $|f''(x)|\le K$ and $a\le x\le b$:
        - Error for trapezoidal: $\color{tomato}|E_T|\le \frac{K(b-a)^3}{12n^2}$
        - Error for mid-point approximation: $\color{tomato}|E_M|\le \frac{K(b-a)^3}{24n^2}$
- Simpson’s rule: Approximate a curve by another parabola
    - Any 3 consecutive points on the curve can form a parabola form $Ax^2+Bx+C$
        
    - Take left, middle and right end points and find the Area, we have
        
        $\int^b_af(x)dx \approx \frac{\Delta x}{3}[{\color{tomato}1}f(x_0)+{\color{tomato}4}f(x_1)+{\color{tomato}2}f(x_2)...+{\color{tomato}2}f(x_{n-2})+{\color{tomato}4}f(x_{n-1})+{\color{tomato}1}f(x_n)]$
        
        - Start with 1, then alternate between 4 and 2 then end with 1
    - Error bound
        
        - For $|f^{4'}(x)|<K$ and $a\le x\le b$:
            - Error for Simpson’s rule: $\color{tomato}|E_S|\le \frac{K(b-a)^5}{180n^4}$

## 6.6: Improper integrals:

- Improper Type 1:
    
    - If the limit exists then improper integral converges, otherwise diverges
    - ex: $\int^\infin _1 \frac 1xdx=\lim\limits_{a\to \infin}\int^a_1 \frac 1xdx=\lim\limits_{a\to \infin}\ln(a)\implies$diverges
- Improper Type 2: discontinuous integrands
    
    - If the limit exists then improper integral converges otherwise diverges
        
    - If there is vertical asymptotes then split the integral:
        
        $\int^b_af(x)dx=\int^c_af(x)dx+\int^b_c f(x)dx$
        

![Screenshot 2022-11-26 at 01.59.35.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/b033e31a-da05-4d40-83b5-de2e3ac39c16/Screenshot_2022-11-26_at_01.59.35.png)

![Screenshot 2022-11-26 at 02.01.43.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/31d2330e-5f5c-4ff1-a125-f95e31a3c032/Screenshot_2022-11-26_at_02.01.43.png)

- Comparison theorem: for $f(x)>g(x)>0$ for $x>a$
    - If $\int^\infin_af(x)dx$ is convergent, then $\int^\infin_ag(x)dx$ converges
    - If $\int^\infin_ag(x)dx$ is divergent, then $\int^\infin_af(x)dx$ diverges

![Screenshot 2022-11-26 at 02.07.49.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/742de7fc-3177-4ab1-a298-83bedc5dc149/Screenshot_2022-11-26_at_02.07.49.png)

$$ \text{Chapter 7: Applications of integration} $$

## 7.1: Area between curves:

- The area of region bounded by curve $f(x)$ and $g(x)$ given $f(x)>g(x)$ is
    - $=\int ^b_a [f(x)-g(x)]dx$
- Area bounded by area to the left and the y-axis
    - $=\int ^d_c [f^{-1}(y)-g^{-1}(y)]dx$

## 7.2: Volumes:

- Definition of volume given the equation of area:
    - $V=\lim\limits_{\Delta\to 0}\sum\limits^n_{i=1}A(x_i^*)\Delta x=\int^b_a A(x)dx=\int^b_a \pi f^2(x)dx$
    - Find $A(x)$ first, which a function of area by cross-slide, generally $A(x)=\pi y^2$

![Screenshot 2022-12-02 at 21.23.33.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/d5c11627-80cb-442a-87da-fc89cb03a99f/Screenshot_2022-12-02_at_21.23.33.png)

- Volume of revolution by cross-section:
    - $V=\color{tomato}\pi\int f^2(x)dx$
    - If revolves around $x-$axis, find each and minus
    - If revolve about $x=-1$, not about the axis
        - Translate the curve so that the line of revolution is seen as the axis
    - If revolves around y-axis, $V=\pi\int x^2.dy$

![Screenshot 2022-10-19 at 13.03.43.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/c4cb3f52-9aeb-4168-be95-4650ba4d9893/Screenshot_2022-10-19_at_13.03.43.png)

## 7.3: Volumes by cylindrical shells method:

- Volume revolving around y-axis, opposite:
    - $\displaystyle V=\lim\limits_{n\to \infin} \sum_{i=1}^n (2\pi \bar x_i ).[f(\bar x_i)]\Delta x=\int^b_a 2\pi {\color{tomato}x} f(x)dx$
- Volume revolving around x-axis:
    - $\displaystyle V=\int^b_a 2\pi {\color{tomato}y} f^{-1}(y)dy$

![Screenshot 2022-12-08 at 09.18.01.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/0dd81dfb-8a9e-4fd6-80e3-18c73a150457/Screenshot_2022-12-08_at_09.18.01.png)

## 7.4: Arc length:

- $L=\lim\limits_{n\to\infin}\sum\limits^n_{i=1}|P_{i-1}.P|$, sum of $n$ straigh lines’ lengths
    - $|P_{i=1}.P|=\sqrt{(\Delta x)^2+(\Delta y)^2}$
- $\color{tomato}\displaystyle L=\int^b_a\sqrt{1+(\frac{dy}{dx})^2}dx$
- If $x=f(y)$ then $L=\int^b_a\sqrt{1+[\frac{dx}{dy}]^2}dy$

![Screenshot 2022-10-19 at 13.35.20.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/a4b776ac-a91e-43b1-8534-4e0b576142d7/Screenshot_2022-10-19_at_13.35.20.png)

## 7.5: Area of a surface of revolution:

- $\displaystyle S=\int ^b_a \color{tomato}2\pi y\sqrt{1+(\frac{dy}{dx})^2}dx$
    - $ds=\sqrt{1+(\frac{dy}{dx})^2}.dx$ or $ds=\sqrt{1+(\frac{dx}{dy})^2}.dx$

## 7.6: Applications:

- Work:
    
    - $\displaystyle F=m.a=m\frac{d^2s}{dt^2}$ and $W=F.d$
        - $lb$ is force in pounds, the weight not mass
    
    $\implies W(\text{from a to b})=\int^b_af(x)dx$ where $f(x)$ is force function
    
    - Hooke’s law: $F=kx$ where $x$ is the extension in meters
    
    $\implies W(\text{to stretch from a m to b m)} = \int^b_akxdx$
    
- ## Hydrostatic pressure and force:
    
- Center of mass
    

![Screenshot 2022-12-08 at 15.59.00.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/6cec521c-1981-4026-9704-995549d1bfe5/Screenshot_2022-12-08_at_15.59.00.png)

- Separable equations:
    - Separate into $h(y).\frac{dy}{dx}=g(x)$ and integrate both sides
    - General solution and particular solution using initial-value
- Mixing problems:
    - $y(t)$ is amount of salt at time $t$, then $y't$ is the rate of salt going in - rate of going out
- Direction field:

$$ \text{Chapter 8: Series} $$

## 8.1: Sequences:

- Notation $\{a_n\}$ or $\{a_n\}^\infin_{n=1}$
- Fibonacci sequence = $\{1,1,2,3,5,8,13,12,....\}$
- $\lim\limits_{n\to\infin}a_n=L$ then the sequence converges, otherwise diverges

![Screenshot 2022-10-19 at 22.11.23.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/a6c114d8-b68b-4ae4-ad26-acf3a0431e26/Screenshot_2022-10-19_at_22.11.23.png)

- Theorem: if $\lim\limits_{n\to \infin}a_n=0\iff \sum\limits_{n=1}^\infin a_n$ is convergent
    
- Theorem: if $\lim\limits_{n\to \infin}a_n\not=0\iff \sum\limits_{n=1}^\infin a_n$ is divergent
    
- A sequence is monotonic if it is either increasing or decreasing
    
    - Use squeeze theorem
- Proof that a sequence is always decreasing by showing that $a_{n+1}<a_n$
    
- Bounded sequence: bounded below and or above making $a_n$ cant go pass that
    
    ![Screenshot 2023-01-09 at 11.09.05.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/abce1562-b4dc-4f41-8431-f60edc370d6c/Screenshot_2023-01-09_at_11.09.05.png)
    

## 8.2: Series:

- Sum of first n terms, $S_n=\sum\limits^n_{i=1} a_i$
    - For geometric sequence: $a_n=a_1.r^{n-1}$
        - $S_n=\frac{a(1-r^n)}{1-r}$, where $|r|<1$
        - $S_\infin = \frac{a}{1-r}$
- Term test: If $\sum_{n=1}^\infin a_n$ converges, $\lim a_n = 0$
    - otherwise $\lim a_n \not= 0$ or doesnt exist then series diverges
- Sum of 2 convergent series converges

## 8.3: The integral and comparison tests:

- Integral test: given $f(x)$ is continuous, positive and globally decreasing on $[1;\infin]$
    - if $\int^\infin_1 f(x)dx$ is convergent then $\sum a_n$ is convergent
    - if $\int^\infin_1 f(x)dx$ is divergent then $\sum a_n$ is divergent
    - *** in the exam
- Comparison test: $\sum a_n$ and $\sum b_n$ are positive sequences with similar mostly similar terms with smaller power terms are different (Example : $\frac{\ln k}{k}>\frac 1k$ or $\frac5{2n^2+4n+3}<\frac 5 {2n^2}$)
    - If every term of $a_n<b_n$ and $\sum b_n$ is convergent then $\sum a_n$ also converges
    - If every term of $a_n>b_n$ and $\sum b_n$ is divergent then $\sum a_n$ also diverges
- Limit comparison test: $\sum a_n$ and $\sum b_n$ are positive sequences
    - $\lim\limits_{n\to\infin}\frac{a_n}{b_n}=0$, the series converges
    - If$\lim\limits_{n\to\infin}\frac{a_n}{b_n}=$ a finite constant, then both sequences either diverge or converge

## 8.4: Other convergence tests:

- Alternating series test: $\sum\limits_{n=1}^\infin(-1)^{n-1}b_n$ has terms alternately positive and negative:
    
    - Is convergent if $b_{n+1}\le b_n$, without sign, for all $n$ and $\lim\limits_{n\to\infin}b_n=0$
    - When $\sum \limits^\infin_{n=0}(-1)^n.[f(x)]^n$ only converges whe f(x)<1
- Absolute convergence: if $\sum |a_n|$ is convergent then $\sum a_n$ is also convergent
    
- The ratio test: $\lim\limits_{n\to \infin}|\frac{a_{n+1}}{a_n}|=L$, next term divided by the current term
    
    - If $L<1$ then the series converge, if $L>1$ then the series diverge
    - If $L=1$ then no conclusion drawn
- The root test:
    
    ![Screenshot 2022-12-29 at 15.47.26.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/89ef50b8-e580-42ed-9297-a82af9c8ff79/Screenshot_2022-12-29_at_15.47.26.png)
    

## 8.5: Power series: ( use ratio test)

- $\sum\limits^\infin_{n=0} c_nx^n=c_0+c_1x+c_2x^2+c_3x^3+....$, an infinite polynomial
- Power series centred at a: $\sum\limits^\infin_{n=0} c_n(x-a)^n=c_0+c_1(x-a)+c_2(x-a)^2+....$
    - Use ratio test: $|\frac{a_{n+1}}{a_n}|= \frac{c_{n+1}(x-a)^{n+1}}{c_n(x-a)^n} <1$ in order to be convergent
    - Only 3 possibilities it can converge:
        1. When $x=a$
        2. The series converges for all $x$
        3. A range $|x-a|<R, R$ is radius of convergence

## 8.6: Representing functions as power series:

- Use the sum to infinity backward, $\frac 1{1-x}=1+x+x^2+x^3+....=\sum\limits^\infin_{n=0} x^n$
    - Example: Express $\frac 1 {1+x^2}=\frac 1 {1--x^2}=\sum (-x^2)^n$
        - Use this if the form is similar to $\frac 1 {1\pm f(x)}$
- Find a power series of $x^3/(x+2)$:
    - $=x^3.\frac{1}{2(1--x/2)}=\frac{x^3} 2 .\sum(-\frac x2 )^n=\sum \frac{(-1)^n}{2^{n+1}}x^{n+3}$
    - As $=\frac {x^3}{2}\sum(\frac{-x}{2})^n{}$, the series converges at $|-x/2|<1$

![Screenshot 2022-10-20 at 15.21.16.png](https://s3-us-west-2.amazonaws.com/secure.notion-static.com/f47872f7-82c4-4409-9640-12f3bdc7b7cb/Screenshot_2022-10-20_at_15.21.16.png)

- Convert from differentiation, integration: derive/integrate on equation to get another serie

not in the exam

## 8.7: Taylor and Maclaurin series:

- Taylor series at a:
    - $f(x)=\sum\limits^\infin_{n=0}\frac{f^n(a)}{n!}(x-a)^n=\color{tomato}f(a)+\frac{f'(a)}{1!}(x-a)+\frac{f''a}{1!}(x-a)+...$
        - where $|x-a|<R$
- Maclaurin series: $f(0)$ from Taylor$=f(0)+\frac{f'(0)}{1!}x+\frac{f''(0)}{2!}x^2+...$
    - Taylor series but $a=0$
- $e=\sum\limits^\infin_{n=0}\frac{x^n}{n!}$
- $T_n, n^{th}$ degree Taylor, slide 60,