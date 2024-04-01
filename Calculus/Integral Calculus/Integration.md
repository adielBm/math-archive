- Suppose that $F(x)$ and $G(x)$ are antiderivatives of $f(x)$ and $g(x)$, respectively

|                         | Formula                                                            |                          |
| ----------------------- | ------------------------------------------------------------------ | ------------------------ |
| Constant Multiplication | $\displaystyle\int cf(x)dx=c\int f(x)dx$                           | $c\in\mathbb{R}$         |
|                         | $\displaystyle\int x^n \, dx=\frac{x^{n+1}}{n+1}+C$                | (for integers $n\geq 0$) |
| Sum                     | $\displaystyle \int [f(x)\pm g(x)]dx= \int f(x)dx\pm \int  g(x)dx$ |                          |
| U-Substitution          | $\displaystyle\int f(g(x)) g'(x)=F(g(x))+C$                        |                          |


- (2.4) Linearity 
	- $\int (\alpha f(x)+\beta g(x)) \, dx=\alpha\int f(x) \, dx+\beta \int g(x) \, dx$

# Integration by parts

- (2.6) Integration by parts
	- $\int f(x)g'(x) \, dx=f(x)g(x) -\int f'(x)g(x) \, dx$ 

- (2.10) Integration by parts for definite integrals
	- $\int ^b_{a}uv' \, dx=uv|^b_{a}-\int ^{b}_{a}u'v \, dx$

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

- $\displaystyle\int a^x \, dx=\frac{a^x}{\ln a}$ (for $a\neq 1,a>0$)
	- $\displaystyle\int e^x \, dx=e^x$
- $\displaystyle\int \frac{1}{x} \, dx = \ln|x| + C$
- $\displaystyle\int \sin x \, dx=-\cos x+C$
- $\displaystyle\int  \cos x\, dx=\sin x+C$
- $\displaystyle\int \frac{1}{\cos^2x} \, dx=\tan x$
- $\displaystyle\int \frac{1}{\sin^2x} \, dx=-\cot x$
- $\displaystyle\int \frac{1}{1 + x^2} \, dx = \arctan(x) + C$
- $\displaystyle\int \frac{1}{\sqrt{1 - x^2}} \, dx = \arcsin(x) + C$
- $\displaystyle\int \ln x \, dx=x\ln x-x+C$
- $\displaystyle\int \tan x \, dx=\ln\left|\cos x\right|+C$
- $\displaystyle\int \cot x\, dx=\ln\left|\sin x\right|+C$
- $\displaystyle\int \frac{1}{\sin x} \, dx=\ln\left|\tan \frac{x}{2}\right|+C$
- $\displaystyle\int \frac{1}{\cos x} \, dx=-\ln\left|\tan \left( \frac{x}{2}-\frac{\pi}{4} \right)\right|+C$



- $\displaystyle\int \frac{1}{\sqrt{ a^2+x^2 }} \, dx=\arcsin \frac{x}{a}+C$





## Examples 

- (2.8a) $\displaystyle\int x\ln x \, dx=\frac{x^2\ln x}{2}-\frac{x^2}{4}+C$
- (2.9) $\displaystyle\int \ln x \, dx=x\ln x-x+C$
- (2.10) $\displaystyle\int \ln^2x \, dx=x\ln^2x-2x\ln x+2x+C$
- (e2.12) $\displaystyle I_{m}=\int \frac{1}{(x^2+a^2)^{m}} \, dx={\begin{cases}I_{1}=\frac{1}{a}\arctan \frac{x}{a}+C \\ I_{m+1}=\frac{1}{2ma^2}\cdot \frac{x}{(x^2+a^2)^m}+\frac{2m-1}{2ma^2}I_{m} \end{cases}}$

___

# Rational Functions

- $\displaystyle \frac{a}{(x-p)^k}$ (where $a,p \in \mathbb{R},\,k \in \mathbb{N}$)
	- $x-p=t$ and $dx=dt$
	- $\displaystyle \int \frac{a}{(x-p)^{k}} \, dx=\begin{cases}{ a\ln|t|+C}  & k=1 \\ a \frac{t^{1-k}}{1-k}+C & k\geq 2 \end{cases}=\begin{cases}{ a\ln|x-p|+C}  & k=1 \\ a \frac{(x-p)^{1-k}}{1-k}+C & k\geq 2 \end{cases}$
- $\displaystyle \frac{ax+b}{(x^2+px+q)^k}$ (where $a,b,p,q \in \mathbb{R},\,k \in \mathbb{N}$ and $x^2+px+q$ has no real roots)
	- Step 1:
		- $\displaystyle ax+b=\frac{a}{2}(2x+p)+b-\frac{ap}{2}$ (note $(2x+p)=(x^2+px+q)'$)
		- $\int \frac{ax+b}{(x^2+px+q)^k} \, dx= \frac{a}{2}\int \frac{2x+p}{(x^2+px+q)} \, dx+\left( b-\frac{ap}{2} \right)\int  \frac{dx}{(x^2+px+q)^k}$
	- Step 2: (evaluate the first integral)
		- $u=x^2+px+q$ and $du=(2x+p)dx$
		- $\displaystyle\int \frac{2x+p}{(x^2+px+q)^{k}} \, dx=\int  \frac{du}{u^k}=\begin{cases}{ \ln|u|+C}  & k=1 \\ \frac{u^{1-k}}{1-k}+C & k\geq 2 \end{cases}$
		- $\displaystyle\int \frac{2x+p}{(x^2+px+q)}dx=\ln(x^2+px+q)+C$
		- $\displaystyle\int \frac{2x+p}{(x^2+px+q)^k}dx=\frac{1}{1-k}(x^2+px+q)^{1-k}+C$ (where $k\geq 2$)
	- Step 3: (evaluate the second integral)
		- $\displaystyle \int  \frac{dx}{(x^2+px+q)^k}$
		- $(x^2+px+q)=\left( x+\frac{p}{2} \right)^2+q-\frac{p^2}{4}$ ([[Completing the square]])
		- $(x^2+px+q)=\left( x+\frac{p}{2} \right)^2+d^2$
		- substitute: $x+\frac{p}{2}=t$ and $dx=dt$
		- $\displaystyle \int  \frac{dx}{(x^2+px+q)^k}=\int  \frac{dx}{\left(\left( x+\frac{p}{2} \right)^2+d^2\right)^k}=\int \frac{dt}{(t^2+d^2)^k}$
		- $\displaystyle I_{k}=\int \frac{dt}{(t^2+d^2)^k}$ (see [[#Examples]] e2.12)
		- $\displaystyle I_{1}=\frac{1}{d}\arctan \frac{t}{d}+C$
		- $\displaystyle I_{k+1}=\frac{1}{2kd^2}\cdot \frac{t}{(t^2+d^2)^k}+\frac{2k-1}{2kd^2}I_k$

### Partial Fraction Decomposition

Decomposition of a [[rational function]] $N(x)/D(x)$ into partial fractions 

1. Divide when improper: When $N(x)/D(x)$ is [[Rational function|improper]] (i.e. $\deg N \geq \deg D$), [[Polynomial Long Division|divide]] the denominator into the numerator to obtain $\displaystyle\frac{N(x)}{D(x)}=Q(x)+\frac{N_{1}(x)}{D(x)}$   where $\deg N_{1}(x)< \deg D(x)$. Then apply Steps 2, 3, and 4 to the proper rational expression $N_{1}(x)/D(x)$
2. Factor denominator: Completely factor the denominator into factors of the form $(px+q)^m$ and $(ax^2+bx+c)^n$ where $ax^2+bx+c$ is irreducible
3. Linear factors: For each factor of the form $(px + q)^m$, the partial fraction decomposition must include the following sum of $m$ fractions $\displaystyle\frac{A_{1}}{(px+q)}+\frac{A_{2}}{(px+q)^2}+\dots+\frac{A_{m}}{(px+q)^m}$
4. Quadratic factors: For each factor of the form $(ax^2 + bx + c)^n$, the partial fraction decomposition must include the following sum of $n$ fractions. $\displaystyle \frac{B_{1}x+C_{1}}{ax^2+bx+c}+\frac{B_{2}x+C_{2}}{(ax^2+bx+c)^2}+\dots+\frac{B_{n}x+C_{n}}{(ax^2+bx+c)^n}$






# Tangent half-angle substitution


- $\displaystyle \sin x={\frac {2t}{1+t^{2}}}$
- $\displaystyle\cos x={\frac {1-t^{2}}{1+t^{2}}}$
- $\displaystyle dx={\frac {2}{1+t^{2}}} dt$


- $\int f(\cos x)\sin x \, dx$ then we can substitute $t=\cos x$
- $\int f(\sin x)\cos x \, dx$ then we can substitute $t=\sin x$


- $\displaystyle\int \sin^{m}x\cos^{n}x \, dx$ ($m,n$ are nonnegative integers)
	- $m$ is odd:
		- $m=2k+1$
		- $\sin ^m x=\sin^{2k+1}x=(\sin^2x)^{k}\sin x=(1-\cos^{2} x)^{k}\sin x$
	- $n$ is odd: 
		- $n=2k+1$
		- $\cos ^n x=\cos^{2k+1}x=(\cos^2x)^{k}\cos x=(1-\sin^{2} x)^{k}\cos x$
	- $m,n$ are even:
		- 



___

- if $\deg p \geq \deg q$ then
	- long div
- if $\deg p < \deg q$
	- פירוק לשברים חלקיים
	- השלמה לריבוע 
	- השלמה לנגזרת


