
- (2.4) Linearity 
	- $\int (\alpha f(x)+\beta g(x)) \, dx=\alpha\int f(x) \, dx+\beta \int g(x) \, dx$


- (2.6) Integration by parts
	- $\int f(x)g'(x) \, dx=f(x)g(x) -\int f'(x)g(x) \, dx$ 
- (2.7) 
	- 

# _u_-substitution

- u-sub
	- $\int f(x) \, dx$
	- $f(x)=g(\varphi (x))\varphi'(x)$
	- $\int g(\varphi(x))\varphi'(x) \, dx=\int g(t) \, dt$

- u-sub (Thomas')
	- $u=g(x)$ is differentiable is a differentiable function whose range is an interval I, and ƒ is continuous on I
	- $\int f(g(x)) \cdot g'(x) \, dx=\int f(t) \, du$


- trigo functions
	- $\int \frac{f'(x)}{f(x)} \, dx=\ln|f(x)|+C$

- version 2
	- $t=\varphi^{-1}(x)$
	- $\int f(x) \, dx=\int f(\varphi(t))\varphi'(t) \, dt$ 


- (2.5)  $f(\alpha x+\beta)$ from (where $\alpha\neq 0$)
	- $\displaystyle\int f(x) \, dx=F(x)+C\implies\displaystyle\int f(\alpha x+\beta) \, dx=\frac{1}{\alpha}F(\alpha x+\beta)+C$ 


- #todo  Substitution in Definite Integrals

# Basic integration formulas

- $\displaystyle\int 0 \, dx=C$
- Cavalieri's quadrature formula
	- $\displaystyle\int x^\alpha \, dx=\frac{x^{\alpha+1}}{\alpha+1}+C$ (for $\alpha\neq -1$)
		- $\displaystyle\int (ax+b)^n \, dx=\frac{(ax+b)^{n+1}}{a(n+1)}+C$ (for $\alpha\neq -1$)
- $\displaystyle\int 1 \, dx=\int  \, dx=x+C$
- $\displaystyle\int \sin x \, dx=-\cos x+C$
- $\displaystyle\int  \cos x\, dx=\sin x+C$
- $\displaystyle\int \frac{1}{\cos^2x} \, dx=\tan x$
- $\displaystyle\int \frac{1}{\sin^2x} \, dx=-\cot x$
- $\displaystyle\int a^x \, dx=\frac{a^x}{\ln a}$ (for $a\neq 1,a>0$)
	- $\displaystyle\int e^x \, dx=e^x$


## Examples 

- (2.8a) $\displaystyle\int x\ln x \, dx=\frac{x^2\ln x}{2}-\frac{x^2}{4}+C$
- (2.9) $\displaystyle\int \ln x \, dx=x\ln x-x+C$
- (2.10) $\displaystyle\int \ln^2x \, dx=x\ln^2x-2x\ln x+2x+C$



___

- if $\deg p \geq \deg q$ then
	- long div
- if $\deg p < \deg q$
	- פירוק לשברים חלקיים
	- השלמה לריבוע 
	- השלמה לנגזרת


