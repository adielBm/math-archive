## Indefinite Integral

The **indefinite integral** of the $f$ with respect to $x$
$${\color{gray} f=F'\implies}\displaystyle\int f(x) dx=F(x)+C$$ 
- (d1.12) $F$ is called an **antiderivative** of $f$ on a given open interval if $F'(x)=f(x)$ for all $x$ in the interval
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

# Definite Integral

## Riemann Sum

- Suppose $f : [a, b] \to \mathbb{R}$ is bounded and $P=\set{x_{0}, x_{1}, x_{2},\dots, x_n}$ is a partition of $[a, b]$ and $\Delta x_i = x_i - x_{i-1}$
	- A **Riemann sum** is represented as: $\displaystyle R(P) = \sum_{i=1}^{n} f(c_i) \cdot \Delta x_i$ where $c_i$ is a chosen point in the $i$-th subinterval $[x_{i-1}, x_i]$
	- **Darboux Sums**: 
		- The **Lower Darboux Sum** 
			- $\displaystyle L(P)=\sum^{n}_{i=1} m_{i}\cdot\Delta x_i$ where $\displaystyle{m_{i}=\inf _{x\in [x_{i-1},x_{i}]}f(x)}$
		- The **Upper Darboux Sum**
			- $\displaystyle U(P)=\sum^{n}_{i=1} M_{i}\cdot\Delta x_i$ where $\displaystyle{M_{i}=\sup _{x\in [x_{i-1},x_{i}]}f(x)}$ 
		- $L(P)\leq U(Q)$ (for any partitions)
		- $\displaystyle\sup_{P}L(P)\leq\inf_{P}U(P)$


>[!notation] $s(P)=L(P)$ and $S(P)=U(P)$

### Darboux Integrals

- Let $\mathcal{P}$ represent all possible [[Interval#Partition|partitions]] over $[ a , b ]$
- The **upper Darboux integral** of $f$ is 
	- $\displaystyle U_{f}= {\overline {\int _{a}^{b}}}f(x)\,\mathrm {d} x=\inf \{ U_{f,P}:P \in \mathcal{P} \}$

- The **lower Darboux integral** of $f$ is
	- $\displaystyle L_{f}= {\underline {\int _{a}^{b}}}f(x)\,\mathrm {d} x=\sup \{ L_{f,P}:P\in \mathcal{P} \}$
-  $L_{f}\leq U_{f}$


- Let $P'$ be a refinement of the partition $P$ of the given interval $[a, b]$ then:
	- $U(P')\leq U(P)$
	- $L(P)\leq L(P')$


- (d1.8) A bounded function $f:[a,b]\to \mathbb{R}$ is called **Reimann-integrable** (or **integrable**) if $\displaystyle {\overline {\int _{a}^{b}}}f(x)\,\mathrm {d} x= {\underline {\int _{a}^{b}}}f(x)\,\mathrm {d} x$, in such case, the common value is called the **definite integral** of $f$ and denote as $\displaystyle\int^{b}_{a} f(x) \, dx$
	- (1.10) $f$ is integrable, if and only if, $\forall \varepsilon>0,\exists P:U_{f,P}-L_{f,P}<\varepsilon$
	- (1.11) $\displaystyle\lim_{ n \to \infty }(U(P_{n})-L(P_{n}))=d_{0}\implies \int_{a}^{b} f(x) \, dx=\lim_{ n \to \infty }U(P_{n})=\lim_{ n \to \infty }L(P_{n})$


## Fundamental Theorem

- **The Fundamental Theorem of Calculus**
	- (Part 1) If $f$ is continuous on $[a,b]$ then:
		- $\displaystyle F(x)=\int_{a}^{x}f(t)  \, dt$ is continuous on $[a,b]$ and differentiable on $(a,b)$.
		- $\displaystyle F'(x)=\frac{d}{dx}\left[ \int_{a}^{x}f(t)  \, dt \right]=f(x)$
	- (Part 2) If $f$ is continuous on $[a,b]$, and $F$ is any antiderivative of $f$ on $[a,b]$, then:
		- $\displaystyle\int^{b}_{a} f(x) \, dx=F(b)-F(a)$
	- (1.13) If $f$ is integrable on $[a,b]$, and $F$ is any antiderivative of $f$ on $[a,b]$, then 
		- $\displaystyle\int^{b}_{a} f(x) \, dx=F(b)-F(a)=F(x) \big|_a^b$

## The Area Problem 

- The problem: finding the area $A$ of the region that lies between the graph of $f$ and the interval $[a, b]$ on the $x$-axis
	- Given a function $f$ that is continuous and nonnegative on an interval $[a, b]$, find the area $A$ of the region that lies between the graph of $f$ and the interval $[a, b]$ on the $x$-axis.
	- Find antiderivative $F$ of $f$ on $[a,b]$, and then $\displaystyle\int^{b}_{a} f(x) \, dx=F(b)-F(a)$ is the area.
	- Rectangle Approximation Method
