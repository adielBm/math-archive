## Indefinite Integral

The **indefinite integral** of the $f$ with respect to $x$
$${\color{gray} f=F'\implies}\displaystyle\int f(x) dx=F(x)+C$$ 
- $F$ is called an **antiderivative** of $f$ on a given open interval if $F'(x)=f(x)$ for all $x$ in the interval
- The process of finding a function from its derivative (i.e. finding an antiderivative) is called **antidifferentiation** (or **integration**)
- A procedure for finding areas via *antidifferentiation* is called the **antiderivative method**

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

- Given a function $f$ that is continuous and nonnegative on an interval $[a, b]$, find the area $A$ of the region that lies between the graph of $f$ and the interval $[a, b]$ on the $x$-axis.


- Rectangle Approximation Method
