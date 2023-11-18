
# Continuous at Point


Definitions

- $f$ is **continuous** in $x_{0}$
- $\displaystyle\lim_{ x \to x_{0} }f(x)=f(x_{0})$
- The **limit** of $f$, as $x$ approaches $x_{0}$, is $f(x_{0})$
- $\displaystyle{\displaystyle (\forall \varepsilon >0)\,(\exists \delta >0)\,(\forall x\in \mathbb {R} )\,(|x-x_{0}|<\delta \implies |f(x)-f(x_{0})|<\varepsilon )}$ 
- (5.4) $\forall(x_{n})^{\infty}_{n=1}~,~\displaystyle\lim_{ n \to \infty}x_{n}=x_{0}\implies\displaystyle\lim_{ n \to \infty }f(x_{n})=f(x_{0})$
- (5.6) $\displaystyle\lim_{ h \to 0 }f(x_{0}+h)=f(x_{0})$
- (5.18) $f$ is **right-** and **left-continuous at** $x_{0}$

Theorems 

- (q5.2) If $f(x)=g(x)$ for all $x$ in some neighborhood of $x_0$, then $f$ is continuous in $x_0$ iff $g$ is continuous in $x_0$ 
- (5.15) if $g$ is continuous in $t_{0}$, and $f$ is continuous in $x_{0}$ where $x_{0}=g(t_{0})$, then $f(g(x))$ is continuous in $t_{0}$

## One Side

- $f$ is **left-continuous at** $x_{0}$
	- $\displaystyle\lim_{ x \to x^{-}_{0} }f(x)=f(x_{0})$
- $f$ is **right-continuous at** $x_{0}$
	- $\displaystyle\lim_{ x \to x^{+}_{0} }f(x)=f(x_{0})$


## Discontinuity point 

- **Removable discontinuity** - $\displaystyle\lim_{ x \to x_{0} }f(x)=L\in\mathbb{R}$, and $f(x_{0})\neq L$ (or $f(x_{0})$ is undefined)
- **Jump discontinuity** (first kind) - $\displaystyle\lim_{ x \to x_{0}^{-} }f(x)\neq\lim_{ x \to x_{0}^{+} }f(x)$
- **Essential discontinuity** (second kind) - At least one of the two one-sided limits does not exist (although can be $\pm\infty$)

# Continuous over an Interval

Definitions ($f$ is defiened in the interval $I$)

- $f$ is continuous over the interval $I$ 
- $f$ is **continuous** on **every inferior point** in $I$, and **right-continuous at** the **left-endpoint** (if exists), and **left-continuous at** the **right-endpoint** (if exists).
- For each sequence $(x_{n})^{\infty}_{n=1}$ of points in the interval $I$. we have $\displaystyle\lim_{ n \to \infty }x_{n}=x_{0}\in{I}\implies{\lim_{ n \to \infty }}f(x_{n})=f(x_{0})$
- $(\forall{x_{0}\in{I}})(\forall{\varepsilon>0})(\exists\delta>0):(\forall{x\in{I}}),~|x-x_{0}|<\delta\implies{|f(x)-f(x_{0})|<\varepsilon}$


Theorems ($f$ is continuous over the interval $I=[a,b]$)

- **Intermediate value theorem** (IVT)
	- $(\displaystyle  {\displaystyle \min(f(a),f(b))<t<\max(f(a),f(b))})\implies{\exists~{c}\in{[a,b]}:f(c)=t}$
- (5.32) **Brouwer's Fixed Point Theorem** (1 dim) - If $f:[a,b]\to[a,b]$ is continuous then $\exists{x}\in{[a,b]}:f(x)=x$
- (5.34) Preservation of intervals - $f(I)= \set{f(x):x\in{I}}$ is either an interval or a point


