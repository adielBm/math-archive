# Antiderivative

- (d1.12) $F$ is called an **antiderivative** of $f$ on some interval if $F'(x)=f(x)$ for all $x$ in that interval

> The process of finding a function from its derivative (i.e. finding an antiderivative) is called **antidifferentiation** (or **integration**). A procedure for finding areas via antidifferentiation is called the **antiderivative method**


# Definite Integral

## by Draboux

### Darboux Sums
	
- The **Lower Darboux Sum** 
	- $\displaystyle L(P)=\sum^{n}_{i=1} m_{i}\cdot\Delta x_i$ where $\displaystyle{m_{i}=\inf _{x\in [x_{i-1},x_{i}]}f(x)}$
- The **Upper Darboux Sum**
	- $\displaystyle U(P)=\sum^{n}_{i=1} M_{i}\cdot\Delta x_i$ where $\displaystyle{M_{i}=\sup _{x\in [x_{i-1},x_{i}]}f(x)}$ 
- $L(P)\leq U(Q)$ (for any partitions)
- $\displaystyle\sup_{P}L(P)\leq\inf_{P}U(P)$
- (1.36) $L(P)\leq \sigma \leq U(P)$

### Upper & Lower Darboux integral

- Let $\mathcal{P}$ represent all possible [[Interval#Partition|partitions]] over $[ a , b ]$
- The **upper Darboux integral** of $f$ is 
	- $\displaystyle U_{f}= {\overline {\int _{a}^{b}}}f(x)\,\mathrm {d} x=\inf \{ U_{f,P}:P \in \mathcal{P} \}$

- The **lower Darboux integral** of $f$ is
	- $\displaystyle L_{f}= {\underline {\int _{a}^{b}}}f(x)\,\mathrm {d} x=\sup \{ L_{f,P}:P\in \mathcal{P} \}$
-  $L_{f}\leq U_{f}$
- Let $P'$ be a refinement of the partition $P$ of the given interval $[a, b]$ then:
	- $U(P')\leq U(P)$
	- $L(P)\leq L(P')$

### Darboux integral

- (d1.8) A bounded function $f:[a,b]\to \mathbb{R}$ is **Darboux-integrable** if $\displaystyle {\overline {\int _{a}^{b}}}f(x)\,\mathrm {d} x= {\underline {\int _{a}^{b}}}f(x)\,\mathrm {d} x$, in such case, the common value is called the **Darboux integral** of $f$ and denote as $\displaystyle\int^{b}_{a} f(x) \, dx$
## by Riemann

### Riemann Sums

Let be a function $f : [a, b] \to \mathbb{R}$ and $P=\set{x_{0}, x_{1}, x_{2},\dots, x_n}$ is a partition of $[a, b]$ and $\Delta x_i = x_i - x_{i-1}$

- (d1.38) $\displaystyle\lambda(P)=\max_{1\leq i\leq n}{\Delta{x_{i}}}$ is the **mesh** (or **norm**) of partition
- (d1.35) The sum $\displaystyle \sigma= R(P) = \sum_{i=1}^{n} f(\xi_i) \cdot \Delta x_i$ where $\xi_i$ is a chosen point in the $i$-th subinterval $[x_{i-1}, x_i]$ is called a **Riemann sum** of $f$ over $[ a , b ]$ with partition $P$

### Riemann Integral

- (d1.39)  $\displaystyle\int ^b_{a}f(x) \, dx=\lim_{ \lambda \to 0 }\sigma$ is the **Riemann integral** 
- (1.40) if $f$ is Riemann-integrable on $[a,b]$ then $f$ is bounded on $[a,b]$

## Equivalence of Definitions

Equivalence of Definitions of Riemann and Darboux Integrals

- (1.42) $f$ is Riemann-integrable iff $f$ Darboux-integrable, in this case Riemann-integral is equal to Darboux-integral

## Theorems & Properties 

- (1.10) $f$ is integrable, if and only if, $\forall \varepsilon>0,\exists P:U_{f,P}-L_{f,P}<\varepsilon$
- (1.11) $\displaystyle\lim_{ n \to \infty }(U(P_{n})-L(P_{n}))=0\implies \int_{a}^{b} f(x) \, dx=\lim_{ n \to \infty }U(P_{n})=\lim_{ n \to \infty }L(P_{n})$
- (1.20,q1.34) Additivity - If $a<c<b$ then $f$ is integrable on $[a,b]$ iff $f$ is ingerable on $[a,c]$ and $[c,b]$. In that case: $\displaystyle\int_a^b f(x) \; dx = \int_a^c f(x) \; dx \, + \int_c^b f(x) \; dx$
- (1.21) Given $f$ is integrable on $[a,b]$, If $c$ and $d$ are numbers such that $a\leq c<d\leq b$, then $f$ is integrable on $[c,d]$
- (1.22a) $\displaystyle\int ^b_{a}f(x) \, dx=-\int ^a_{b}f(x) \, dx$
- (1.22b) $\displaystyle\int ^a_{a}f(x) \, dx=0$
- Given $f$ and $g$ are integrable on $[a,b]$ :
	- (1.24) Linearity
		- $\displaystyle\int ^b_{a}cf(x) \, dx=c\int ^b_{a}f(x) \, dx$
		- $\displaystyle\int ^b_{a}(-f(x)) \, dx=-\int ^b_{a}f(x) \, dx$
		- $\displaystyle\int ^b_{a}(f(x)\pm g(x)) \, dx=\int ^b_{a} f(x)\, dx\pm\int ^b_{a} g(x)\, dx$
		- If $f,g$ are continuous then, $\displaystyle A =\left|{\int^{x_{2}}_{x_{1}}(f(x)-g(x))  \, dx}\right|$ represents the area between the curves $f(x)$ and $g(x)$ over the interval $[x_1, x_2]$
	- (1.26) If $\forall x \in[a,b], f(x)\leq g(x)$ then $\displaystyle\int ^b_{a}f(x) \, dx\leq\int ^b_{a}g(x) \, dx$
- (1.25) If $f(x)=g(x)$ for every $x$ excluding finite number of points on $[a,b]$, then, if $g$ integrable on $[a,b]$ then $f$ integrable on $[a,b]$, and $\int ^b_{a}f(x) \, dx=\int ^b_{a}g(x) \, dx$
- $\forall a,b,c$ we have $\displaystyle\int ^b_{a}c \, dt=c(b-a)$ 
- if $f$ is integrable on an interval where $a$ and $b$ are its endpoints and $|f(x)|\leq M$ for all $x$ in that interval, then $\displaystyle\left|\int^b_{a} f(t) \, dt\right|\leq M|b-a|$
- (1.41) if $f$ is Darboux-integrable on $[a,b]$, then $\displaystyle \lim_{ \lambda(P) \to 0 }(S(P)-s(P))=0$
# Indefinite Integral

- (d2.1) The collection of all antiderivatives called the **indefinite integral** of the $f$ with respect to $x$ and denote by: 
	- $\displaystyle\int f(x) dx= \{ F(x):F'(x)=f(x),x \in I \}$
		- The symbol $\int$ is an **integral sign**
		- The function $f$ is the **integrand** of the integral
		- $x$ is the **variable of integration**
- (2.2) if $F$ is an antiderivative of $f$ then $\int f(x) \, dx=\{ G:G=F+c,c \in \mathbb{R} \}$. (or shortly, $F'=f\implies \int f(x) \, dx=F(x)+C$)


- (d1.30) if $f$ is integrable on $[a,b]$ and $c \in [a,b]$ then the function $\displaystyle F_{c}(x)=\int ^x_{c}f(t) \, dt$ which is defined on $[a,b]$ is an **indefinite integral** of $f$ on $[a,b]$ 


### Properties

- Suppose that $F(x)$ and $G(x)$ are antiderivatives of $f(x)$ and $g(x)$, respectively

|                         | Formula                                                            |                          |
| ----------------------- | ------------------------------------------------------------------ | ------------------------ |
| Constant Multiplication | $\displaystyle\int cf(x)dx=c\int f(x)dx$                           | $c\in\mathbb{R}$         |
|                         | $\displaystyle\int x^n \, dx=\frac{x^{n+1}}{n+1}+C$                | (for integers $n\geq 0$) |
| Sum                     | $\displaystyle \int [f(x)\pm g(x)]dx= \int f(x)dx\pm \int  g(x)dx$ |                          |
| U-Substitution          | $\displaystyle\int f(g(x)) g'(x)=F(g(x))+C$                        |                          |
# Theorems

### Sufficient Conditions for Integrabletly

- sufficient conditions for integrabletly of $f$ on $[a,b]$
	- (1.11) $\displaystyle\lim_{ n \to \infty }(U(P_{n})-L(P_{n}))=0$
	- (1.15) if $f$ is weakly monotonic on $[a,b]$
	- (1.17) if $f$ is bounded and piecewise monotone on $[a,b]$
	- (1.18) if $f$ is continuous (thus bounded) on $[a,b]$ 
	- (1.19) if $f$ is bounded and continuous on $[a,b]$ (possibly expect finites number of discontinuity points), then

### Outcomes of Integrable Function



- If $f$ is integrable on $[a,b]$ then: 
	- (1.13, הנוסחה היסודית, Newton–Leibniz theorem) 
		- if $F$ is any antiderivative of $f$ on $[a,b]$, then $\displaystyle\int^{b}_{a} f(x) \, dx=F(b)-F(a)=F(x) \big|_a^b$
	- (1.27) $|f|$ is also integrable on $[a,b]$
	- (1.32) every indefinite integral of $f$ on $[a,b]$ is continuous on $[a,b]$
	- (1.31) the difference of each two indefinite integrals of $f$ on $[a,b]$ is constant
	- (1.34) if $f$ has an antiderivative function on $[a,b]$ then the indefinite integral $\displaystyle\int ^x_{c}f(t) \, dt$ is an antiderivative of $f$ on $[a,b]$

### Outcomes of Continuous Function

- if $f$ is continuous on $[a,b]$ then:
	- (1.18) $f$ is integrable (thus bounded) on $[a,b]$ 
	- (1.29 - MVT for Integrals) $\exists c \in[a,b]:\displaystyle\int ^b_{a}f(x) \, dx=f(c)(b-a)$
	- (q1.57) for all $c \in [a,b]$, the indefinite integral $\displaystyle\int ^x_{c}f(t) \, dt$ is an antiderivative of $f$ on $[a,b]$
	- (1.33) The Fundamental Theorem of Calculus 
		- $\displaystyle F_{a}(x)=\int_{a}^{x}f(t)  \, dt$ is differentiable on $[a,b]$ and 
		- $\displaystyle F'_{a}(x)=\frac{d}{dx}\left[ \int_{a}^{x}f(t)  \, dt \right]=f(x)$
	- (1.33') The Fundamental Theorem of Calculus
		- $f$ has an antiderivative function on $[a,b]$
		- every antiderivative function of $f$ on $[a,b]$ is of the form $\displaystyle\int ^x_{a}f(t) \, dt+C$ where $C$ is some real number

# Applications
## The Area Problem 

- Given a continuous function $f$
	- $\displaystyle\int^{b}_{a} |f(x)| \, dx$ is the area of of the region that lies between the graph of $f$ and the interval $[a, b]$ on the $x$-axis

 