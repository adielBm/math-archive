# Differentiability 

> $\operatorname{dom}(f)$ contains an open interval $I$ containing $x_{0}$

- $f(x)$ is **differentiable at a point** $x_{0}\in\operatorname{dom}(f)$
-  The limit $\displaystyle  L=\lim _{h\to 0}{\frac {f(x_{0}+h)-f(x_{0})}{h}}=\lim_{x\to{x_{0}}}{\frac{f(x)-f(x_{0})}{x-x_{0}}}$ exists
- $(\forall \varepsilon > 0 )(\exists\delta>0)\forall h\left(0<|h|<\delta\implies \left|L - \frac{f(x_{0}+h)-f(x_{0})}{h}\right| < \varepsilon \right)$
- #todo  $\exists{A}\in\mathbb{R} : f(x_{0}+h)-f(x_{0})=Ah+\alpha(h)h$ where $\displaystyle\lim_{ h \to 0 }\alpha(h)=0$

# Derivative

- Derivative Function - $\displaystyle f'(x)=\frac{df}{dx}=\lim _{h\to 0}{\frac {f(x+h)-f(x)}{h}}$

> $f(x)$ is **differentiable at a point** $x_{0}\in\operatorname{dom}(f)$

- Derivative of $f$ at the point $x_{0}$ is $f'(x_{0})$
	- $\displaystyle f'(x_{0})=\lim _{h\to 0}{\frac {f(x_{0}+h)-f(x_{0})}{h}}=\lim_{x\to{x_{0}}}{\frac{f(x)-f(x_{0})}{x-x_{0}}}$
	- $f'(x_{0})$ is the **slope of the tangent line** to the graph of $f$ at the point $x_{0}$
	- $f'(x_{0})$ is the **instantaneous rate of change** of $f$ with respect to $x$ at $x_{0}$

> Notation $\displaystyle f'(x_{0})=\frac{df}{dx}(x_{0}) = \left.{\frac {df}{dx}}\right|_{x=x_{0}}$


> [!note] Rate of Change 
> - The **average rate of change** of $y=f(x)$ with respect to $x$ over the interval $[x_{0},x_{1}]$ is $\frac{\Delta y}{\Delta x}=\frac{f(x_{1})-f(x_{0})}{x_{1}-x_{0}}=\frac{f(x_{0}+h)-f(x_{0})}{h}$ (where $h\neq 0$) 
> - The **instantaneous rate of change** of $f$ with respect to $x$ at $x_{0}$ is the derivative $f'(x_{0})=\displaystyle\lim _{h\to 0}{\frac {f(x_{0}+h)-f(x_{0})}{h}}$. (provided the limit exists)


- (7.9) if $f$ is differentiable at $x_{0}$, then it continuous at $x_{0}$

## Derivative Rules

- Sum Rule $(f+g)'(x_{0})=f'(x_{0})+g'(x_{0})$ 
- Product Rule $(fg)'={fg'}+{f'g}$
	- Constant Multiple Rule $(cf)'(x_{0})=c\cdot f'(x_{0})$
	- (7.17) $(f^{n})'(x)=nf^{n-1}(x)\cdot f'(x)$ 
	- (7.20) Power Rule $(x^n)'=nx^{n-1}$ ( #todo  integer $n\neq 0$ )
- Quotient Rule $\displaystyle\left( \frac{f}{g} \right)'(x_{0})=\frac{f'g-fg'}{g^2}$ 
	- (7.19) **Reciprocal rule**
		- $\displaystyle\left( \frac{1}{f} \right)'=\frac{{-f'}}{f^2}$
		- $\displaystyle\frac{d}{dx}\left[ \frac{1}{f(x)} \right]=\frac{{-f'(x)}}{[f(x)]^2}$
- Chain Rule 
	- $(f(g(x)))'=f'(g(x))\cdot g'(x)$
	- $(f(g(h(x))))'=f'(g(h(x))) \cdot g'(h(x)) \cdot h'(x)$
	- $\displaystyle  {\frac {dz}{dx}}={\frac {dz}{dy}}\cdot {\frac {dy}{dx}}$


## Root Function 

- $(\sqrt{ x })'=\frac{1}{2\sqrt{ x }}$
- $(\sqrt{ f(x) })'=\frac{f'(x)}{2\sqrt{ f(x) }}$

## Inverse functions

> assuming: $f$ is *continuous* and *monotonic* on $I$

- (7.27) $\big(f^{−1}\big)'(x)=\frac{1}{f'\big(f^{−1}(x)\big)}$

- if $f'(x_{0})=0$ then $(f^{-1})'(f(x_{0}))$ is undefined 

## Trigonometric Functions 

- $\sin'(x)=\cos x$
- $\cos'(x)=-\sin x$
- $\tan'(x)=\sec^2x=\frac{1}{\cos^2 x}=1+\tan^{2}x$
- $\cot'(x)=-\frac{1}{\sin^2x}$

## Inverse trigonometric functions

- $\arcsin'(x)=\frac{1}{\sqrt{1-x^2}}$
- $\arccos'(x)=\frac{-1}{\sqrt{1-x^2}}$
- $\arctan'(x)=\frac{1}{1-x^2}$
- $\text{arccot}'(x)=\frac{-1}{\sqrt{1-x^2}}$

## Exponential functions

- $(a^x)'=a^x\cdot{\ln a}$
	- Natural Exponential - $(e^x)'=e^x$

## Logarithmic functions

- $(\log_{a}x)'=\frac{1}{x\ln a}$
	- The natural logarithm function - $\ln'(x)=\frac{1}{x}$

# Differentiability on Interval

- $f$ is continuous on $[a,b]$, differentiable on the $(a,b)$
	- **Rolle's theorem** - $f(a)=f(b)\implies\exists c\in(a,b):f'(c )=0$
	- **Mean value theorem** (MVT, Lagrange) - $\exists c\in(a,b):f'(c )=\frac{{f(b)-f(a)}}{b-a}$

- $f$ is *continuous* and *differentiable* on $(a,b)$
	- (8.7, q7.12) $(\forall{x\in{(a,b)},f'(x)=0})\iff$ $f$ is constant on $(a,b)$ 
	- (q8.28) $(\forall{x\in{(a,b)},f'(x)\geq 0})\iff$ $f$ is **increasing** on $(a,b)$
		- (8.18) $(\forall{x\in{(a,b)},f'(x)>0})\implies$ $f$ is **strictly increasing** on $(a,b)$
	- $(\forall{x\in{(a,b)},f'(x)\leq0})\iff$ $f$ is **decreasing** on $(a,b)$
		- (8.18) $(\forall{x\in{(a,b)},f'(x)<0})\implies$ $f$ is **strictly decreasing** on $(a,b)$

> Note: $a$ and $b$ can be $-\infty$ and $\infty$ (resp.)

> By (q8.25) if $f$ is continuous on $[a,b]$ and **monotonic** on $(a,b)$ then $f$ is **monotonic** on $[a,b]$ 

- $f$ and $g$ is continuous on $[a,b]$, differentiable on the $(a,b)$
	- **Cauchy's mean value theorem** - if $\forall{x\in{(a,b)}},\, g'(x)\neq 0$, then:
		- $g(a)\neq g(b)$
		- $\displaystyle\exists{c\in{(a,b)}}:\frac{f'(c)}{g'(c)}=\frac{f(b)-f(a)}{g(b)-g(a)}$

> MVT is special case of Cauchy's MVT when $g(x)=x$


- **Darboux's theorem** - $f$ is differentiable on the $(a,b)$ then $f'$ has the intermediate value property.
	- 

- **Constant Difference Theorem** #not-in-course If $f$ and $g$ are differentiable on an interval, and if $f'(x)=g'(x)$ for all $x$ in that interval, then $f − g$ is constant on the interval; that is, there is a constant k such that $f(x) − g(x) = k$ or, equivalently, $f(x) = g(x) + k$ for all $x$ in the interval. 


### Concavity #todo 

- The graph of a differentiable function y = ƒ(x) is
	- **concave up** on an open interval $I$ if $f'$ is increasing on I
	- **concave down** on an open interval $I$ if $f'$ is decreasing on I
- A point $(c,f(c))$ where the graph of a function has a tangent line and where the concavity changes is a **point of inflection**
- The Second Derivative Test for Concavity #todo 
- At a point of inflection (c, ƒ(c)), either ƒ″(c) = 0 or ƒ″(c) fails to exist.

# Second Derivative 

- (8.23) if $f'(x_{0})=0$ and $f''(x_{0})\neq 0$ then $x_{0}$ is local extremum of $f$
	- if $f''(x_{0})> 0$ then $x_{0}$ is local minimum of $f$
	- if $f''(x_{0})< 0$ then $x_{0}$ is local maximum of $f$

