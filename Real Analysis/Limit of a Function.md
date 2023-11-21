
- The **limit** of $f$, as $x$ approaches $x_{0}$, is $L$
- $\displaystyle\lim_{ x \to x_{0} }f(x)=L$ 
- ((ε, δ)-definition of limit. Cauchy) 
	- $\displaystyle  {\displaystyle (\forall \varepsilon >0)\,(\exists \delta >0)\,(\forall x\in \mathbb {R} )\,(0<|x-x_{0}|<\delta \implies |f(x)-L|<\varepsilon )}$ 
- (The Sequential Criterion for a Limit of a Function. Heine) 
	- $\forall(x_{n})^{\infty}_{n=1}~~(\displaystyle\lim_{ n \to \infty}(x_{n})=x_{0})\land(\forall{n\in\mathbb{N}},x_{n}\neq x_{0})\implies\displaystyle\lim_{ n \to \infty }f(x_{n})=L$
- (**left** & **right**-hand limit)
	- $\displaystyle\lim_{x\to{x_{0}}^{-}}f(x)=\displaystyle\lim_{x\to{x_{0}}^{+}}f(x)=L$
- (4.40) $\displaystyle\lim_{h\to 0}{f(x_0+h)}=L$

Theorems



- (4.31) **Uniqueness** of the limit of function 
	- $(f(x) \underset{n \to x_{0}}{\longrightarrow} L\land{f(x) \underset{n \to x_{0}}{\longrightarrow} M})\implies{L=M}$
- (4.33) Limit of **Linear Function** 
	- Let $f$ a linear function then for each $x_{0}\in\mathbb{R}$, we have $\displaystyle\lim_{ x \to {x_{0}} }f(x)=f(x_{0})$
- (4.34) if $\displaystyle\lim_{x\to{x_0}}{f(x)}$ is defined, and $f(x)=g(x)$ for each $x$ such that $x_0-\delta<x\neq{x_0}<{x_0}+\delta$, then $\displaystyle\lim_{x\to{x_0}}{f(x)}=\lim_{x\to{x_0}}{g(x)}$
- (4.43) Squeeze theorem for functions
	- $\Big(f(x)\leq g(x)\leq h(x)\Big)\land\Big({\displaystyle\lim_{ x \to x_{0} }f(x)=\lim_{ x \to x_{0} }h(x)=L}\Big)\implies{\displaystyle\lim_{ x \to x_{0} }g(x)=L}$



| Limit Laws       |                                                                                                                   |
| ---------------- | ----------------------------------------------------------------------------------------------------------------- |
| Sum / Difference | $\displaystyle\lim _{x\to x_{0}}(f(x)\pm g(x))=\displaystyle \lim _{x\to x_{0}}f(x)\pm\lim _{x\to x_{0}}g(x)$     |
| Product          | $\displaystyle\lim _{x\to x_{0}}(f(x)\cdot g(x))=\displaystyle \lim _{x\to x_{0}}f(x)\cdot\lim _{x\to x_{0}}g(x)$ |
|                  | $\displaystyle\lim _{x\to x_{0}}(f(x)\cdot c)=\displaystyle \lim _{x\to x_{0}}f(x)\cdot c$                        |
|                  |  $\displaystyle\lim _{x\to x_{0}}(f(x))^n=\Big(\displaystyle \lim _{x\to x_{0}}f(x)\Big)^{n}$                                                                                                                  |
| Quotient          | $\displaystyle\lim _{x\to x_{0}}(f/g)(x)=\displaystyle \lim _{x\to x_{0}}f(x)/\lim _{x\to x_{0}}g(x)$ where $\displaystyle\lim _{x\to x_{0}}g(x)\neq 0$ |



- (q4.62) $\displaystyle\lim_{x\to0}{f(x)}=L\implies\lim_{x\to 0}{f(x^2)}=L$
-  (q4.63) $\displaystyle\lim_{x\to0}{f(x)}=\lim_{x\to 0}{f(xk)}$  (where $k\neq 0$ and the limits exists)
- Limit of a Composite Function: $\displaystyle\lim_{ t \to t_{0} }f(g(t))=\displaystyle\lim_{ x \to {(\lim_{ t \to t_{0} }g(t))} }f(x)$
 
   

### Examples

- (4.44a) $\displaystyle\lim_{ x \to 0 }\sin x=0$
- (4.44b) $\displaystyle\lim_{ x \to 0 }\cos x=1$
- (4.45) $\displaystyle\lim_{ x \to 0 }{\frac{\sin x}{x}}=\lim_{ x \to 0 }{\frac{x}{\sin x}}=1$


## One-Sided Limits

- $L$ is the **right-hand limit** of $f$ at $x_{0}$
	- $\displaystyle\lim_{x\to{x_{0}}^{+}}f(x)=L$
	- $\displaystyle  {\displaystyle (\forall \varepsilon >0)\,(\exists \delta >0)\,(\forall x\in \mathbb {R} )\,(x\in(x_{0},x_{0}+\delta)\implies{f(x)}\in(L-\varepsilon,L+\varepsilon))}$ 
	- Sequential Criterion (*Heine*)
		- $\forall(x_{n})^{\infty}_{n=1}~~(\displaystyle\lim_{ n \to \infty }(x_{n})=x_{0})\land(\forall{n\in\mathbb{N}},x_{n}>x_{0})\implies\displaystyle\lim_{ n \to \infty }f(x_{n})=L$
- $L$ is the **left-hand limit** of $f$ at $x_{0}$
	- $\displaystyle\lim_{x\to{x_{0}}^{-}}f(x)=L$
	- $\displaystyle  {\displaystyle (\forall \varepsilon >0)\,(\exists \delta >0)\,(\forall x\in \mathbb {R} )\,(x\in(x_{0}-\delta,x_{0})\implies{f(x)}\in(L-\varepsilon,L+\varepsilon))}$
	- Sequential Criterion (*Heine*)
		- $\forall(x_{n})^{\infty}_{n=1}~~(\displaystyle\lim_{ n \to \infty }(x_{n})=x_{0})\land(\forall{n\in\mathbb{N}},x_{n}<x_{0})\implies\displaystyle\lim_{ n \to \infty }f(x_{n})=L$

## Infinite limits

- $\displaystyle\lim_{ x \to x_{0} }f(x)=\infty$ 
- $\displaystyle  {\displaystyle (\forall M\in\mathbb{R})\,(\exists \delta >0)\,(\forall x\in \mathbb {R} )\,(0<|x-x_{0}|<\delta \implies f(x)>M )}$
	- (Note: It's sufficient to ensure for $M>0$.)
- $\forall(x_{n})^{\infty}_{n=1}~~(\displaystyle\lim_{ n \to \infty }(x_{n})=x_{0})\land(\forall{n\in\mathbb{N}},x_{n}\neq x_{0})\implies\displaystyle\lim_{ n \to \infty }f(x_{n})=\infty$
- $\displaystyle\lim_{x\to{x_{0}}^{-}}f(x)=\infty=\displaystyle\lim_{x\to{x_{0}}^{+}}f(x)$

> $\displaystyle\lim_{ x \to x_{0} }f(x)=-\infty$ (or one-sided Limits) defined the same, just replace $f(x)>m$ with $f(x)<m$ 

### One-Sided Limits

- $\infty$ is the **right-hand limit** of $f$ at $x_{0}$
	- $\displaystyle\lim_{x\to{x_{0}}^{+}}f(x)=\infty$
	- $\displaystyle  {\displaystyle (\forall M\in\mathbb{R})\,(\exists \delta >0)\,(\forall x\in \mathbb {R} )\,(x\in(x_{0},x_{0}+\delta) \implies f(x)>M )}$
	- $\forall(x_{n})^{\infty}_{n=1}~~(\displaystyle\lim_{ n \to \infty }(x_{n})=x_{0})\land(\forall{n\in\mathbb{N}},x_{n}> x_{0})\implies\displaystyle\lim_{ n \to \infty }f(x_{n})=\infty$
- $\infty$ is the **left-hand limit** of $f$ at $x_{0}$
	- $\displaystyle\lim_{x\to{x_{0}}^{-}}f(x)=\infty$
	- $\displaystyle  {\displaystyle (\forall M\in\mathbb{R})\,(\exists \delta >0)\,(\forall x\in \mathbb {R} )\,(x\in(x_{0}-\delta,x_{0}) \implies f(x)>M )}$
	- $\forall(x_{n})^{\infty}_{n=1}~~(\displaystyle\lim_{ n \to \infty }(x_{n})=x_{0})\land(\forall{n\in\mathbb{N}},x_{n}< x_{0})\implies\displaystyle\lim_{ n \to \infty }f(x_{n})=\infty$

### Arithmetic of Infinite limits

- $\infty+\infty=\infty$
- $\infty+r=\infty$
- $\infty\cdot\infty=\infty$
- $\infty\cdot{r}=\infty$
- $1/\infty=0$
- $1/0^{+}=0$
- $\displaystyle\lim_{ x \to x_{0} }(f(x))=\infty \iff\displaystyle\lim_{ x \to x_{0} }(-f(x))=-\infty$

## Limits at Infinity

- $L$ is the **limit** of $f$ at $\infty$
	- $\displaystyle\lim_{ x \to \infty }f(x)=L$
	- $\displaystyle  {\displaystyle (\forall \varepsilon >0)\,(\exists M)\,(\forall x\in \mathbb {R} )\,(x>M \implies |f(x)-L|<\varepsilon )}$ 
	- $\forall(x_{n})^{\infty}_{n=1}~~\displaystyle\lim_{ n \to \infty}x_{n}=\infty\implies\displaystyle\lim_{ n \to \infty }f(x_{n})=L$
- $L$ is the **limit** of $f$ at $-\infty$
	- $\displaystyle\lim_{ x \to -\infty }f(x)=L$
	- $\displaystyle  {\displaystyle (\forall \varepsilon >0)\,(\exists M)\,(\forall x\in \mathbb {R} )\,(x<M \implies |f(x)-L|<\varepsilon )}$ 
	- $\forall(x_{n})^{\infty}_{n=1}~~\displaystyle\lim_{ n \to \infty}x_{n}=-\infty\implies\displaystyle\lim_{ n \to \infty }f(x_{n})=L$

- #todo $\infty$ is the **limit** of $f$ at $\infty$
- #todo $\infty$ is the **limit** of $f$ at $-\infty$