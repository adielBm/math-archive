
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


___

#### #todo 

- (5.40) if $f$ is increasing on neighborhood of $x_{0}$, then the one-side limits $\displaystyle\lim_{ x \to x_{0}^{-} }f(x)$ and $\displaystyle\lim_{ x \to x_{0}^{+} }f(x)$ exist and $\displaystyle\lim_{ x \to x_{0}^{-} }f(x)\leq f(x_{0})\leq\lim_{ x \to x_{0}^{+} }f(x)$
- (5.41) **Discontinuity of Monotonic Function** is Jump Discontinuity
	- if $f$ is monotonic in $(a,b)$ and let $x_{0}\in{(a.b)}$ be a discontinuity point, then it's the *jump discontinuity* point
- (5.42) $f$ is monotonic on $I$. if the interval image $f(I)$ is also an interval, then $f$ is continuous on $I$
- $f$ is monotonic and continuous on $I$ then: 
	- (5.43) there exist a inverse fucntion $f^{-1}$ whose domain is $f(I)$ and its image is $I$ which $f^{-1}$ itself is monotonic and continuous on $f(I)$. ($f^{-1}$ is increasing if $f$ is decreasing, and vice versa)

___

## Extreme (maximum & minimum)

- $f$ is defined on an interval $I=\operatorname {dom} (f)$
	- **Global Extreme**
		- **Extremum point**: $x_{0}\in{I}$ is a **maximum point** (resp. **minimum point**) on $I$ of $f$ if $\displaystyle  \forall (x\in I),\,f(x_{0})\geq f(x)$ (resp. $f(x_{0})\leq f(x)$)
			- **Extremum value:**  In this case, $f(x_{0})$ is called the **maximum** (resp. **minimum**) **(value)** on $I$, and $f$ is said to have a maximum (resp. minimum) (value) on $I$ at a point $x_{0}$
	- **Local Extreme** (מקסימום/מינימום מקומי)
		- **Local Extremum point**: $x_{0}\in{I}$ is a **local maximum point** (resp. **local minimum point**) at $I$ if there exists a neighborhood $N_{\varepsilon}(x_{0})$ such that $\forall x \in N_{\varepsilon}(x_{0}),f(x_{0})\geq f(x)$ (resp. $f(x)\geq f(x_{0})$) (in both cases נקודת קיצון)
			- In this case, $f(x_{0})$ is called a **local maximum (value)** (resp. **local minimum (value)**) of $f$ at a point $x_{0}$. (in both cases $f(x_{0})$ is also called **local extremum value**, ערך קיצון)


- (8.3) A Extremum point on $I$ is either a local extremum point of $f$ or an endpoint of $I$
- (8.4) **Fermat's theorem** (interior extremum theorem) - if $x_{0}$ is a local extremum point of $f$, and $f$ is differentiable at $x_{0}$, then $f'(x_{0})=0$
- Global Extreme points can be, either 
	- endpoints of $I$, or 
	- inferior points of $I$, in which $f$ is *not* differentiable, or 
	- inferior points of $I$, in which the derivative of $f$ is $0$


- $x_{0}$ is a **critical point** of $f$ if either $f'(x_{0})=0$ or $f'(x_{0})$ is undefined
	- $x_{0}$ is a **stationary point** of $f$ if $f'(x)=0$
- (8.19) if $x_{0}$ is local extremum (interior point) then $x_{0}$ a critical point




> Some say *relative* instead of *local*, and *absolut* instead of *global*
# Exponential Functions

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

# Logarithmic Functions

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