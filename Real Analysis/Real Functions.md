
- A **real fucntion** is a function whose domain and codomain are sets of real numbers

## Monotonicity

- $f$ is a real function that defined on interval $I$
	- $f$ is **increasing** if $\forall x_{1},x_{2}\in{I},~~ x_{1}<x_{2}\implies{f(x_{1})\leq f(x_{2})}$
		- $f$ is **strictly increasing** if $\forall x_{1},x_{2}\in{I},~~ x_{1}<x_{2}\implies{f(x_{1})< f(x_{2})}$
	- $f$ is **decreasing** if $\forall x_{1},x_{2}\in{I},~~ x_{1}<x_{2}\implies{f(x_{1}) \geq f(x_{2})}$
		- $f$ is **strictly decreasing** if $\forall x_{1},x_{2}\in{I},~~ x_{1}<x_{2}\implies{f(x_{1})> f(x_{2})}$
	- $f$ is **monotonic** if it's increasing or decreasing


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
- (5.43) $f$ is monotonic and continuous on $I$ then there exist a inverse fucntion $f^{-1}$ whose domain is $f(I)$ and its image is $I$ which $f^{-1}$ itself is monotonic and continuous on $f(I)$. ($f^{-1}$ is increasing of $f$ is decreasing, and vice versa)

___


## Extremum (maximum & minimum)

- $x_{0}\in{X}$ is a **global maximum** point of function $\displaystyle  f:X\to \mathbb {R} ,$ if  $\displaystyle  (\forall x\in X)\,f(x_{0})\geq f(x)$
- $x_{0}\in{X}$ is a **global minimum** point of function $\displaystyle  f:X\to \mathbb {R} ,$ if  $\displaystyle  (\forall x\in X)\,f(x_{0})\leq f(x)$

#todo 
- $x_{0}$ is a **local maximum** point of function
- $x_{0}$ is a **local minimum** point of function 

