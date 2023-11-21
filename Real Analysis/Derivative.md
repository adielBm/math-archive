
## Differentiability 
	
> $\operatorname{dom}(f)$ contains an open interval $I$ containing $x_{0}$

- $f(x)$ is **differentiable at a point** $x_{0}\in\operatorname{dom}(f)$
-  The limit $\displaystyle  L=\lim _{h\to 0}{\frac {f(x_{0}+h)-f(x_{0})}{h}}=\lim_{x\to{x_{0}}}{\frac{f(x)-f(x_{0})}{x-x_{0}}}$ exists
- $(\forall \varepsilon > 0 )(\exists\delta>0)\forall h\left(0<|h|<\delta\implies \left|L - \frac{f(x_{0}+h)-f(x_{0})}{h}\right| < \varepsilon \right)$
- #todo  $\exists{A}\in\mathbb{R} : f(x_{0}+h)-f(x_{0})=Ah+\alpha(h)h$ where $\displaystyle\lim_{ h \to 0 }\alpha(h)=0$

## Derivative

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

### Derivative Rules

- Derivative Sum Rule $(f+g)'(x_{0})=f'(x_{0})+g'(x_{0})$ 
- Derivative Product Rule $(fg)'={fg'}+{f'g}$
	- Derivative Constant Multiple Rule $(cf)'(x_{0})=c\cdot f'(x_{0})$
	- $(f^{n})'(x)=nf^{n-1}(x)\cdot f'(x)$
- Derivative Quotient Rule $\displaystyle\left( \frac{f}{g} \right)'(x_{0})=\frac{f'g-fg'}{g^2}$ 



