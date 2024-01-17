
- A **real fucntion** is a function whose domain and codomain are sets of real numbers

## Monotonicity

- $f$ is a real function that defined on interval $I$
	- $f$ is **(weakly) increasing** if $\forall x_{1},x_{2}\in{I},~~ x_{1}<x_{2}\implies{f(x_{1})\leq f(x_{2})}$
		- $f$ is **(strictly) increasing** if $\forall x_{1},x_{2}\in{I},~~ x_{1}<x_{2}\implies{f(x_{1})< f(x_{2})}$
	- $f$ is **(weakly) decreasing** if $\forall x_{1},x_{2}\in{I},~~ x_{1}<x_{2}\implies{f(x_{1}) \geq f(x_{2})}$
		- $f$ is **(strictly) decreasing** if $\forall x_{1},x_{2}\in{I},~~ x_{1}<x_{2}\implies{f(x_{1})> f(x_{2})}$
	- $f$ is **monotonic** if it's increasing or decreasing

>in this course monotonic is strictly monotonic

## Bounded function 

- $f$ is a real function that defined on a set $D$ is called **bounded** on $D$ if $f(D)$ is **bounded**.

## Limits of Bounded Monotonic Function 

- (5.39) **Bounded Monotonic Function** - $f$ is **monotonic** and defined on open interval $(a,b)$.
	- $f$ is **bounded** on an open interval $(a,b)$, then both $\displaystyle\lim_{ x \to b^{-} }f(x)$ and $\displaystyle\lim_{ x \to a^{+} }f(x)$ exist (finite)
		- if $f$ is **increasing** then 
			- $\displaystyle\lim_{ x \to b^{-} }f(x)=\sup f\big((a,b)\big)$ 
			- $\displaystyle\lim_{ x \to a^{+} }f(x)=\inf f\big((a,b)\big)$ 
		- if $f$ is **decreasing** then 
			- $\displaystyle\lim_{ x \to b^{-} }f(x)=\inf f\big((a,b)\big)$ 
			- $\displaystyle\lim_{ x \to a^{+} }f(x)=\sup f\big((a,b)\big)$ 
	- if $f$ is **not bounded above**
		- if $f$ is **increasing** then 
			- $\displaystyle\lim_{ x \to b^{-} }f(x)=+\infty$ 
		- if $f$ is **decreasing** then 
			- $\displaystyle\lim_{ x \to a^{+} }f(x)=+\infty$ 
	- if $f$ is **not bounded below**
		- if $f$ is **increasing** then 
			- $\displaystyle\lim_{ x \to a{+} }f(x)=-\infty$ 
		- if $f$ is **decreasing** then 
			- $\displaystyle\lim_{ x \to b^{-} }f(x)=-\infty$ 

## Extreme (maximum & minimum)

- $f$ is defined on an interval $I=\text {dom} (f)$
	- **Global Extreme**
		- **Extremum point**: $x_{0}\in{I}$ is a **maximum point** (resp. **minimum point**) on $I$ of $f$ if $\displaystyle  \forall (x\in I),\,f(x_{0})\geq f(x)$ (resp. $f(x_{0})\leq f(x)$)
			- **Extremum value:**  In this case, $f(x_{0})$ is called the **maximum** (resp. **minimum**) **(value)** on $I$, and $f$ is said to have a maximum (resp. minimum) (value) on $I$ at a point $x_{0}$
	- **Local Extreme** (מקסימום/מינימום מקומי)
		- **Local Extremum point**: $x_{0}\in{I}$ is a **local maximum point** (resp. **local minimum point**) at $I$ if there exists a neighborhood $N_{\varepsilon}(x_{0})$ such that $\forall x \in N_{\varepsilon}(x_{0}),f(x_{0})\geq f(x)$ (resp. $f(x)\geq f(x_{0})$) (in both cases נקודת קיצון)
			- In this case, $f(x_{0})$ is called a **local maximum (value)** (resp. **local minimum (value)**) of $f$ at a point $x_{0}$. (in both cases $f(x_{0})$ is also called **local extremum value**, ערך קיצון)

- $x_{0}$ is called a **critical point** of $f$ if either $f'(x_{0})=0$ or $f'(x_{0})$ is undefined
	- $x_{0}$ is called a **stationary point** of $f$ if $f'(x)=0$

> Some say *relative* instead of *local*, and *absolut* instead of *global*


### Theorems

- (8.3) A extremum point on $I$ is either a local extremum point of $f$ or an endpoint of $I$
- **Fermat's theorem** - equivalence theorems:
	- (8.4) let $x_{0}$ a local extremum point of $f$. if $f$ is differentiable at $x_{0}$, then $f'(x_{0})=0$
	- (8.19) if $x_{0}$ is a local extremum point of $f$, then, $f$ is not differentiable at $x_{0}$, **xor**, ($f$ is differentiable and $f'(x_{0})=0$)   
- If $x_{0}$ is a global extremum of $f$, then one of the following is true: 
	- $x_{0}$ is an endpoint of $I$ 
	- $f$ is not differentiable at $x_{0}$ 
	- $x_{0}$ is a stationary point of $f$, (i.e. $f'(x_{0})=0$)
- (8.21) Let $f$ be a function that is continuous at a point $x_0$ and differentiable in a punctured neighborhood $N_{\varepsilon}(x_0)$ of $x_0$.
	* If the derivative $f'$ changes its sign as it passes through $x_0$:
		* If the sign change is from $-$ to $+$, then $x_0$ is a local minimum point of $f$.
		* If the sign change is from $+$ to $-$, then $x_0$ is a local maximum point of $f$.
	* If there exists a punctured neighborhood of $x_0$ in which the sign of $f'$ is constant, then $x_0$ is not an extremum point of $f$.

## Misc 

- (5.40) if $f$ is increasing on neighborhood of $x_{0}$, then the one-side limits $\displaystyle\lim_{ x \to x_{0}^{-} }f(x)$ and $\displaystyle\lim_{ x \to x_{0}^{+} }f(x)$ exist and $\displaystyle\lim_{ x \to x_{0}^{-} }f(x)\leq f(x_{0})\leq\lim_{ x \to x_{0}^{+} }f(x)$
- (5.41) **Discontinuity of Monotonic Function** is Jump Discontinuity
	- if $f$ is monotonic in $(a,b)$ and let $x_{0}\in{(a.b)}$ be a discontinuity point, then it's the *jump discontinuity* point
- (5.42) $f$ is monotonic on $I$. if the interval image $f(I)$ is also an interval, then $f$ is continuous on $I$
- $f$ is monotonic and continuous on $I$ then: 
	- (5.43) there exist a inverse fucntion $f^{-1}$ whose domain is $f(I)$ and its image is $I$ which $f^{-1}$ itself is monotonic and continuous on $f(I)$. ($f^{-1}$ is increasing if $f$ is decreasing, and vice versa)


# Classification

## Elementary functions

### Algebraic functions

Algebraic functions are functions that can be expressed as the solution of a polynomial equation with integer coefficients.

- Polynomials
- Rational functions
- nth root

### Elementary Transcendental functions

Transcendental functions are functions that are not algebraic.
#### Exponential Functions

- $f(x)=a^x$ where $a>0$
	- $\text{dom}(f)=\mathbb{R}$
	- $f$ is continuous on $\mathbb{R}$
	- one-to-one function
	- x-intercept: none
	- y-intercept:  $(0,1)$
	- $\text{Im}f=(0,\infty)$
	- Inverse Function $f^{-1}=\log_{a}(x)$ (where $a\neq 1$)
	- Limit  
		- (Increasing) $a>1\implies$ 
			- $\displaystyle\lim_{ x \to -\infty }f(x)=0$
			- $\displaystyle\lim_{ x \to \infty }f(x)=\infty$
		- (Decreasing) $0<a<1\implies$ 
			- $\displaystyle\lim_{ x \to -\infty }f(x)=\infty$
			- $\displaystyle\lim_{ x \to \infty }f(x)=0$
	- [[Derivative#Examples|Derivative]]



#### Logarithmic Functions

- $f(x)=\log_{a}(x)$ where $a>0$ and $a\neq 1$
	- $\text{dom}f=(0,\infty)$
	- $\text{Im}f=\mathbb{R}$
	- $f$ is continuous on $(0,\infty)$
	- one-to-one function
	- X-intercept: $(1,0)$
	- Y-intercept: none
	- Asymptotes
		- Vertical asymptote at $x=0$
		- Horizontal asymptote as $x$ approaches infinity
	- Inverse Function $f^{-1}=a^x$
	- Limit  
		- (Increasing) $a>1\implies$ 
			- $\displaystyle\lim_{ x \to 0^+}f(x)= -\infty$
			- $\displaystyle\lim_{ x \to \infty }f(x)=\infty$
		- (Decreasing) $0<a<1\implies$ 
			- $\displaystyle\lim_{ x \to 0^+ }f(x)=\infty$
			- $\displaystyle\lim_{ x \to \infty }f(x)=-\infty$
	- [[Derivative#Examples|Derivative]]


#### Periodic functions

##### Trigonometric Functions 



