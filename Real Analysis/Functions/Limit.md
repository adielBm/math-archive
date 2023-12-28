# Finite Limit

### Definitions

- The **limit** of $f$, as $x$ approaches $x_{0}$, is $L$
- $\displaystyle\lim_{ x \to x_{0} }f(x)=L$ 
- ((ε, δ)-definition of limit. Cauchy) 
	- $\displaystyle  {\displaystyle (\forall \varepsilon >0)\,(\exists \delta >0)\,(\forall x\in \mathbb {R} )\,(0<|x-x_{0}|<\delta \implies |f(x)-L|<\varepsilon )}$ 
- (The Sequential Criterion for a Limit of a Function. Heine) 
	- $\forall(x_{n})^{\infty}_{n=1}~~(\displaystyle\lim_{ n \to \infty}(x_{n})=x_{0})\land(\forall{n\in\mathbb{N}},x_{n}\neq x_{0})\implies\displaystyle\lim_{ n \to \infty }f(x_{n})=L$
- (**left** & **right**-hand limit) (4.47)
	- $\displaystyle\lim_{x\to{x_{0}}^{-}}f(x)=\displaystyle\lim_{x\to{x_{0}}^{+}}f(x)=L$
- (4.40) $\displaystyle\lim_{h\to 0}{f(x_0+h)}=L$

### Theorems

- (4.31) **Uniqueness** of the limit of function 
	- $(f(x) \underset{n \to x_{0}}{\longrightarrow} L\land{f(x) \underset{n \to x_{0}}{\longrightarrow} M})\implies{L=M}$
- (4.33) Limit of **Linear Function** 
	- Let $f$ a linear function then for each $x_{0}\in\mathbb{R}$, we have $\displaystyle\lim_{ x \to {x_{0}} }f(x)=f(x_{0})$
- (4.34) if $\displaystyle\lim_{x\to{x_0}}{f(x)}$ is defined, and $f(x)=g(x)$ for each $x$ such that $x_0-\delta<x\neq{x_0}<{x_0}+\delta$, then $\displaystyle\lim_{x\to{x_0}}{f(x)}=\lim_{x\to{x_0}}{g(x)}$
- (4.43) Squeeze theorem for functions
	- $\Big(f(x)\leq g(x)\leq h(x)\Big)\land\Big({\displaystyle\lim_{ x \to x_{0} }f(x)=\lim_{ x \to x_{0} }h(x)=L}\Big)\implies{\displaystyle\lim_{ x \to x_{0} }g(x)=L}$
- if $\displaystyle  {\displaystyle (\forall \varepsilon >0)\,(\exists \delta >0)\,(\forall x\in \mathbb {R} )\,(0<|x-x_{0}|<\delta \implies |f(x)-L|<K\varepsilon )}$ where $K$ is a positive real number that does not depend on $\varepsilon$ or $x$ then $\displaystyle\lim_{ x \to x_{0} }f(x)=L$ 
### Arithmetic

| Limit Laws |  |
| ---- | ---- |
| Sum / Difference | $\displaystyle\lim _{x\to x_{0}}(f(x)\pm g(x))=\displaystyle \lim _{x\to x_{0}}f(x)\pm\lim _{x\to x_{0}}g(x)$ |
| Product | $\displaystyle\lim _{x\to x_{0}}(f(x)\cdot g(x))=\displaystyle \lim _{x\to x_{0}}f(x)\cdot\lim _{x\to x_{0}}g(x)$ |
|  | $\displaystyle\lim _{x\to x_{0}}(f(x)\cdot c)=\displaystyle \lim _{x\to x_{0}}f(x)\cdot c$ |
|  | $\displaystyle\lim _{x\to x_{0}}(f(x))^n=\Big(\displaystyle \lim _{x\to x_{0}}f(x)\Big)^{n}$ |
| Quotient | $\displaystyle\lim _{x\to x_{0}}(f/g)(x)=\displaystyle \lim _{x\to x_{0}}f(x)/\lim _{x\to x_{0}}g(x)$ where $\displaystyle\lim _{x\to x_{0}}g(x)\neq 0$ |
| Composite Function | $\displaystyle\lim_{ t \to t_{0} }f(g(t))=\displaystyle\lim_{ x \to {(\lim_{ t \to t_{0} }g(t))} }f(x)$ |


- (q4.62) $\displaystyle\lim_{x\to0}{f(x)}=L\implies\lim_{x\to 0}{f(x^2)}=L$
-  (q4.63) $\displaystyle\lim_{x\to0}{f(x)}=\lim_{x\to 0}{f(xk)}$  (where $k\neq 0$ and the limits exists)


# One-Sided Limits

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


# Infinite limits

- $\displaystyle\lim_{ x \to x_{0} }f(x)=\infty$ 
- $\displaystyle  {\displaystyle (\forall M\in\mathbb{R})\,(\exists \delta >0)\,(\forall x\in \mathbb {R} )\,(0<|x-x_{0}|<\delta \implies f(x)>M )}$
	- (Note: It's sufficient to ensure for $M>0$.)
- $\forall(x_{n})^{\infty}_{n=1}~~(\displaystyle\lim_{ n \to \infty }(x_{n})=x_{0})\land(\forall{n\in\mathbb{N}},x_{n}\neq x_{0})\implies\displaystyle\lim_{ n \to \infty }f(x_{n})=\infty$
- $\displaystyle\lim_{x\to{x_{0}}^{-}}f(x)=\infty=\displaystyle\lim_{x\to{x_{0}}^{+}}f(x)$

> $\displaystyle\lim_{ x \to x_{0} }f(x)=-\infty$ (or one-sided Limits) defined the same, just replace $f(x)>m$ with $f(x)<m$ 

## One-Sided Limits

- $\infty$ is the **right-hand limit** of $f$ at $x_{0}$
	- $\displaystyle\lim_{x\to{x_{0}}^{+}}f(x)=\infty$
	- $\displaystyle  {\displaystyle (\forall M\in\mathbb{R})\,(\exists \delta >0)\,(\forall x\in \mathbb {R} )\,(x\in(x_{0},x_{0}+\delta) \implies f(x)>M )}$
	- $\forall(x_{n})^{\infty}_{n=1}~~(\displaystyle\lim_{ n \to \infty }(x_{n})=x_{0})\land(\forall{n\in\mathbb{N}},x_{n}> x_{0})\implies\displaystyle\lim_{ n \to \infty }f(x_{n})=\infty$
- $\infty$ is the **left-hand limit** of $f$ at $x_{0}$
	- $\displaystyle\lim_{x\to{x_{0}}^{-}}f(x)=\infty$
	- $\displaystyle  {\displaystyle (\forall M\in\mathbb{R})\,(\exists \delta >0)\,(\forall x\in \mathbb {R} )\,(x\in(x_{0}-\delta,x_{0}) \implies f(x)>M )}$
	- $\forall(x_{n})^{\infty}_{n=1}~~(\displaystyle\lim_{ n \to \infty }(x_{n})=x_{0})\land(\forall{n\in\mathbb{N}},x_{n}< x_{0})\implies\displaystyle\lim_{ n \to \infty }f(x_{n})=\infty$
- $-\infty$ is the **right-hand limit** of $f$ at $x_{0}$
	- $\displaystyle\lim_{x\to{x_{0}}^{+}}f(x)=-\infty$
	- $\displaystyle  {\displaystyle (\forall M\in\mathbb{R})\,(\exists \delta >0)\,(\forall x\in \mathbb {R} )\,(x_{0}<x<x_{0}+\delta) \implies f(x)<M )}$
	- $\forall(x_{n})^{\infty}_{n=1}~~(\displaystyle\lim_{ n \to \infty }(x_{n})=x_{0})\land(\forall{n\in\mathbb{N}},x_{n}> x_{0})\implies\displaystyle\lim_{ n \to \infty }f(x_{n})=-\infty$
- $-\infty$ is the **left-hand limit** of $f$ at $x_{0}$
	- $\displaystyle\lim_{x\to{x_{0}}^{-}}f(x)=-\infty$
	- $\displaystyle  {\displaystyle (\forall M\in\mathbb{R})\,(\exists \delta >0)\,(\forall x\in \mathbb {R} )\,(x_{0}-\delta<x<x_{0}) \implies f(x)<M )}$
	- $\forall(x_{n})^{\infty}_{n=1}~~(\displaystyle\lim_{ n \to \infty }(x_{n})=x_{0})\land(\forall{n\in\mathbb{N}},x_{n}< x_{0})\implies\displaystyle\lim_{ n \to \infty }f(x_{n})=-\infty$

## Arithmetic of Infinite limits

- $\infty+\infty=\infty$
- $\infty+r=\infty$
- $\infty\cdot\infty=\infty$
- $\infty\cdot{r}=\infty$
- $1/\infty=0$
- $1/0^{+}=\infty$
- $\displaystyle\lim_{ x \to x_{0} }(f(x))=\infty \iff\displaystyle\lim_{ x \to x_{0} }(-f(x))=-\infty$

# Limits at Infinity

- $L$ is the **limit** of $f$ at $\infty$
	- $\displaystyle\lim_{ x \to \infty }f(x)=L$
	- ${\displaystyle (\forall \varepsilon >0)\,(\exists M)\,(\forall x\in \mathbb {R} )\,(x>M \implies |f(x)-L|<\varepsilon )}$
	- $\forall(x_{n})^{\infty}_{n=1}~~\displaystyle\lim_{ n \to \infty}x_{n}=\infty\implies\displaystyle\lim_{ n \to \infty }f(x_{n})=L$
- $L$ is the **limit** of $f$ at $-\infty$
	- $\displaystyle\lim_{ x \to -\infty }f(x)=L$
	- $\displaystyle  {\displaystyle (\forall \varepsilon >0)\,(\exists M)\,(\forall x\in \mathbb {R} )\,(x<M \implies |f(x)-L|<\varepsilon )}$ 
	- $\forall(x_{n})^{\infty}_{n=1}~~\displaystyle\lim_{ n \to \infty}x_{n}=-\infty\implies\displaystyle\lim_{ n \to \infty }f(x_{n})=L$

-  $\infty$ is the **limit** of $f$ at $\infty$
	- $\displaystyle\lim_{ x \to \infty }f(x)=\infty$
	- $\displaystyle  {\displaystyle (\forall M_{1} \in\mathbb{R})\,(\exists M_{2} \in\mathbb{R})\,(\forall x\in \mathbb {R} )\,(x>M_{2} \implies f(x)>M_{1} )}$ 
	- $\forall(x_{n})^{\infty}_{n=1}~~\displaystyle\lim_{ n \to \infty}x_{n}=\infty\implies\displaystyle\lim_{ n \to \infty }f(x_{n})=\infty$


- #todo $\infty$ is the **limit** of $f$ at $-\infty$


- Limit at Infinity of **Rational Function** $\displaystyle \frac{f(x)}{g(x)}=\frac{a_{n}x^n+\dots+a_{0}}{b_{m}x^m+\dots+b_{0}}$
	- $\displaystyle\deg(f)<\deg(g)\implies\displaystyle\lim_{x\to\infty}\frac{\frac{a_nx^n}{x^m}+...+\frac{a_0}{x^m}}{\frac{b_mx^m}{x^m}+...+\frac{b_0}{x^m}}=\frac{0+...+0}{b_m+...+0}=\frac{0}{b_m}=0$
	- $\displaystyle\deg(f)=\deg(g)\implies\displaystyle\lim_{x\to\infty}\frac{\frac{a_nx^n}{x^n}+...+\frac{a_0}{x^n}}{\frac{b_nx^n}{x^n}+...+\frac{b_0}{x^n}}=\frac{a_{n}+...+0}{b_n+...+0}=\frac{a_{n}}{b_n}$
	- $\displaystyle\deg(f)>\deg(g)\implies\lim_{x\rightarrow \infty}\frac{f(x)}{g(x)}=\pm \infty$ (depending on the sign of $\frac{a_{n}}{b_{m}}$)

# L'Hôpital's rule

- Suppose $f$ and $g$ are differentiable and $g'(x)\neq 0$ on an open interval $I$ that contains $a$ (except possibly at $a$). 
	- "$\displaystyle\frac{0}{0}$" - If $\displaystyle\lim_{ x \to x_{0} }f(x)=\lim_{ x \to x_{0} }g(x)=0$, then $\displaystyle\lim_{ x \to x_{0} }\frac{f(x)}{g(x)}=\lim_{ x \to x_{0} }\frac{f'(x)}{g'(x)}$ (if the limit on the right side exists (finite, or is $\infty$ or $-\infty$)


	- "$\displaystyle\frac{\infty}{\infty}$" - If $\displaystyle\lim_{ x \to x_{0} }f(x)=\lim_{ x \to x_{0} }g(x)=0$, then $\displaystyle\lim_{ x \to x_{0} }\frac{f(x)}{g(x)}=\lim_{ x \to x_{0} }\frac{f'(x)}{g'(x)}$ (if the limit on the right side exists (finite, or is $\infty$ or $-\infty$)

> There's similar theorems for one-side limits, limit *at-infinity*, 



# Examples


- (e4.31) $\displaystyle\lim_{ x \to \infty }\sqrt{ x }=\infty$



- (4.44a) $\displaystyle\lim_{ x \to 0 }\sin x=0$
- (4.44b) $\displaystyle\lim_{ x \to 0 }\cos x=1$
- (4.45) $\displaystyle\lim_{ x \to 0 }{\frac{\sin x}{x}}=\lim_{ x \to 0 }{\frac{x}{\sin x}}=1$

- $\displaystyle\lim_{ x \to 0 }\frac{\tan x}{x}=1$
- $\displaystyle\lim_{ x \to 0 }\frac{\tan^2 x}{x}=0$
- $\displaystyle\lim_{ x \to 0 }{\frac{\sin (cx)}{x}}=c$
- $\displaystyle\lim_{ x \to 0 }{\frac{\sin (x)}{cx}}=\frac{1}{c}$
- $\displaystyle\lim_{x \to 0}{\frac{\arcsin{x}}{x}}=\lim_{x \to 0}{\frac{\arctan{x}}{x}}=1$
- $\displaystyle\lim_{x\to\infty} (x \sin(1/x)) = 1$
- (q4.85c) $\displaystyle\lim_{ x \to \infty }f(x)=\lim_{ x \to 0^+ }f(1/x)$ (assuming $f$ defined on $(M,\infty)$)


- $(\cos{x})^{\sin x}$
	- $\displaystyle\lim_{ x \to 0 }(\cos{x})^{\sin x}=$ #todo see e6.3 page 179


- $x$
	- (q4.82a) $\displaystyle\lim_{ x \to \infty } {x}=\infty$
	- $\displaystyle\lim_{ x \to x_{0} } {x}=x_{0}$

- $x^c$
	- $c>0$
		- $\displaystyle\lim_{ x \to \infty }x^c=\infty$
		- $\displaystyle\lim_{ x \to 0^+ }x^c=0$



- $c^x$
	- $c>1$
		- $\displaystyle\lim_{ x \to \infty }c^x=\infty$
		- $\displaystyle\lim_{ x \to -\infty }c^x=0$
		- $\displaystyle\lim_{ x \to x_{0} }c^x=c^{x_{0}}$ #todo 
	- $0<c<1$
		- $\displaystyle\lim_{ x \to \infty }c^x=0$
		- $\displaystyle\lim_{ x \to -\infty }c^x=\infty$

- $\ln x$
	- $\displaystyle\lim_{ x \to \infty }\ln x=\infty$
	- $\displaystyle\lim_{ x \to 0^+ }\ln x=-\infty$


- $\displaystyle\lim_{ x \to 0^+ }x^x=1$

- $\displaystyle\frac{1}{x-x_{0}}$
	- $\displaystyle\lim_{x\to x_{0}} \frac{1}{x-x_{0}}$ *does **not** exist* $\impliedby\displaystyle\lim_{x\to x_{0}^{+}} \frac{1}{x-x_{0}}=\infty\land\lim_{x\to x_{0}^{-}} \frac{1}{x-x_{0}}=-\infty$
	- $\displaystyle\lim_{ x \to \infty } \frac{1}{x-x_{0}}=0$
	- $\displaystyle\frac{1}{x}$ (Special Case $x_{0}=0$)
		- $\displaystyle\lim_{x\to {0}} \frac{1}{x}$ *does **not** exist* $\impliedby\displaystyle\lim_{x\to {0}^{+}} \frac{1}{x}=\infty\land\lim_{x\to {0}^{-}} \frac{1}{x}=-\infty$
		- (q4.78) $\displaystyle\lim_{ x \to \infty } \frac{1}{x}=0$


- $\displaystyle\left( 1+\frac{1}{x} \right)^x$
	- (6.16) $\displaystyle\lim_{ x \to \infty }\left( 1+\frac{1}{x} \right)^x=e$
	- (6.17) $\displaystyle\lim_{ x \to -\infty }\left( 1+\frac{1}{x} \right)^x=e$
- $(1+x)^{1/x}$
	- (6.18) $\displaystyle\lim_{ x \to 0 }(1+x)^{1/x}=e$


- $\displaystyle\frac{x^r}{a^x}$ (assuming $a>1$, and $r\in\mathbb{R}$)
	- $\displaystyle\lim_{ x \to \infty }\frac{x^r}{a^x}=0$

# Asymptotes

- The vertical line $x=x_{0}$ is a **vertical asymptote** of the function $y = f(x)$ if
	- $\displaystyle \lim _{x\to x_{0}^{-}}f(x)=\pm \infty$, or
	- $\displaystyle \lim _{x\to x_{0}^{+}}f(x)=\pm \infty$ 

-  The horizontal line $y=c$ is a **horizontal asymptote** of the function $y=f(x)$ if
	- $\displaystyle \lim _{x\rightarrow -\infty }f(x)=c$, or 
	- $\displaystyle \lim _{x\rightarrow +\infty }f(x)=c$

- The straight line $y = mx + n$ is an **oblique asymptote** of the function $y=f(x)$ if 
	- $\displaystyle\lim _{x\to -\infty }\left[f(x)-(mx+n)\right]=0$, or
	- $\displaystyle \lim _{x\to +\infty }\left[f(x)-(mx+n)\right]=0$ 


