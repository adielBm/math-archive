## Indefinite Integral

The **indefinite integral** of the $f$ with respect to $x$
$${\color{gray} f=F'\implies}\displaystyle\int f(x) dx=F(x)+C$$ 
- $F$ is called an **antiderivative** of $f$ on a given open interval if $F'(x)=f(x)$ for all $x$ in the interval
- The process of finding a function from its derivative (i.e. finding an antiderivative) is called **antidifferentiation** (or **integration**)
- A procedure for finding areas via *antidifferentiation* is called the **antiderivative method**

### Properties 

- Suppose that $F(x)$ and $G(x)$ are antiderivatives of $f(x)$ and $g(x)$, respectively

|  | Formula |  |
| ---- | ---- | ---- |
| Constant Multiplication | $\displaystyle\int cf(x)dx=c\int f(x)dx$ | $c\in\mathbb{R}$ |
|  | $\displaystyle\int x^n \, dx=\frac{x^{n+1}}{n+1}+C$ | (for integers $n\geq 0$) |
| Sum | $\displaystyle \int [f(x)\pm g(x)]dx= \int f(x)dx\pm \int  g(x)dx$ |  |
| U-Substitution | $\displaystyle\int f(g(x)) g'(x)=F(g(x))+C$ |  |

## Definite Integral

- $f(x)$ is continuous on $[a ,b]$
- Divide $[a, b]$ into $n$ subintervals of width $\Delta x=\frac{{b-a}}{n}$
- $x^*_i$ as sample point for each interval

$$\displaystyle{\int^{b}_{a} f(x) \, dx=\lim_{ n \to \infty }\sum^{n}_{i=1} f(x^{*}_{i})\cdot\Delta{x}}$$


- **The Fundamental Theorem of Calculus**
	- (Part 1) If $f$ is continuous on $[a,b]$ then:
		- $\displaystyle F(x)=\int_{a}^{x}f(t)  \, dt$ is continuous on $[a,b]$ and differentiable on $(a,b)$.
		- $\displaystyle F'(x)=\frac{d}{dx}\left[ \int_{a}^{x}f(t)  \, dt \right]=f(x)$
	- (Part 2) If $f$ is continuous on $[a,b]$, and $F$ is any antiderivative of $f$ on $[a,b]$, then:
		- $\displaystyle\int^{b}_{a} f(x) \, dx=F(b)-F(a)$

## The Area Problem 

- A **partition** of an interval $[a,b]$ is a set $P=\set{x_{0}, x_{1}, x_{2},\dots, x_n}$ where $a=x_{0} < x_{1} < x_{2} < \dots < x_{n}=b$
	- Every interval of the form $[x_{i}, x_{i} + 1]$ is referred to as a **subinterval** of the partition $x$.
	- A **refinement** of the partition $P$ of the given interval $[a, b]$ is a partition $Q$ that contains all the points of $P$ and possibly some other points as well. (the partition $Q$ is said to be "finer" than $P$)
		- Given two partitions, $P$ and $Q$, one can always form their **common refinement**, denoted $P∨Q$, which consists of all the points of $P$ and $Q$, in increasing order

### Riemann Sum

- Suppose $f : [a, b] \to \mathbb{R}$ is bounded and $P=\set{x_{0}, x_{1}, x_{2},\dots, x_n}$ is a partition of $[a, b]$ and $\Delta x_i = x_i - x_{i-1}$
	- A **Riemann sum** is represented as: $\displaystyle R(f, P) = \sum_{i=1}^{n} f(c_i) \cdot \Delta x_i$ where $c_i$ is a chosen point in the $i$-th subinterval $[x_{i-1}, x_i]$
	- **Darboux Sums**: 
		- The **Lower Darboux Sum** 
			- $\displaystyle L(f,P)=\sum^{n}_{i=1} m_{i}\cdot\Delta x_i$ where $\displaystyle{m_{i}=\inf _{x\in [x_{i-1},x_{i}]}f(x)}$
		- The **Upper Darboux Sum**
			- $\displaystyle U(f,P)=\sum^{n}_{i=1} M_{i}\cdot\Delta x_i$ where $\displaystyle{M_{i}=\sup _{x\in [x_{i-1},x_{i}]}f(x)}$ 
		- $L(P)\leq U(Q)$ (for any partitions)
		- $\displaystyle\sup_{P}L(f,P)\leq\inf_{P}U(f,P)$



- Let $P'$ be a refinement of the partition $P$ of the given interval $[a, b]$ then:
	- $U(P')\leq U(P)$
	- $L(P)\leq L(P')$


- A bounded function $f:[a,b]\to \mathbb{R}$ is called **Reimann-integrable** (or **integrable**) if $\displaystyle\sup_{P}L(f,P)=\inf_{P}U(f,P)$, in such case, this value called the **(Reimann) integral** of $f$ and denote as $\displaystyle\int^{b}_{b} f(x) \, dx$




- Given a function $f$ that is continuous and nonnegative on an interval $[a, b]$, find the area $A$ of the region that lies between the graph of $f$ and the interval $[a, b]$ on the $x$-axis.

- Find antiderivative $F$ of $f$ on $[a,b]$, and then $\displaystyle\int^{b}_{a} f(x) \, dx=F(b)-F(a)$ is the area.



- Rectangle Approximation Method
