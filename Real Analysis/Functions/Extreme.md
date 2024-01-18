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
- (8.21) **First Derivative Test for Local Extreme** - Let $f$ be a function that is continuous at a point $x_0$ and differentiable in a punctured neighborhood $N_{\varepsilon}(x_0)$ of $x_0$.
	* If the derivative $f'$ changes its sign as it passes through $x_0$:
		* If the sign change is from $-$ to $+$, then $x_0$ is a local minimum point of $f$.
		* If the sign change is from $+$ to $-$, then $x_0$ is a local maximum point of $f$.
	* If there exists a punctured neighborhood of $x_0$ in which the sign of $f'$ is constant, then $x_0$ is not an extremum point of $f$.
