Power Series (6.2)

- Convergence Radius of Power Series
- Behavior of Power Series at Points $|x|=R$
- Taylor Series
- Expansion of the Function $(1+x)^\alpha$ into Power Series

- A **power series** (centered at $a$) is a series of the form $$\sum_{n=0}^{\infty}c_n(x-a)^n$$ where $(c_n)$ is a sequence of real numbers and $a$ is a real number.
	- The number $a$ is called the **center** of the power series.
	- The constants $c_0,c_1,c_2,\dots$ are called the **coefficients** of the power series.


- Given a power series $\sum_{n=0}^{\infty}c_n(x-a)^n$. Then there are only three possibilities:
	- (i) The series converges only when $x=a$.
	- (ii) The series converges for all $x$.
	- (iii) There exists a positive number $R$ such that the series converges if $|x-a|<R$ and diverges if $|x-a|>R$. 
		- The number $R$ is called the **radius of convergence** of the power series.
		- Interval of convergence #todo
- (6.10) Given a power series $\sum_{n=0}^{\infty}c_n(x)^n$. Let's denote $C=\displaystyle\limsup_{n\to\infty}\sqrt[n]{|c_n|}$.
	- $R=\begin{cases}0&\text{if }C=\infty\\\infty&\text{if }C=0\\\frac{1}{C}&\text{if }0<C<\infty\end{cases}$ is called the **radius of convergence** of the power series.
	- (a.) The series converges absolutely for all real number $x$ in $(-R,R)$.
	- (b.) The series converges uniformly on every closed interval $[-r,r]$ where $0<r<R$.
- (6.11) Given a power series $\sum_{n=0}^{\infty}c_n(x)^n$. If the limit $R=\displaystyle\lim_{n\to\infty}\left|\frac{c_{n}}{c_{n+1}}\right|$ exists, (finite or infinite), then the radius of convergence is $R$.
- (6.12) Given a power series $\sum_{n=0}^{\infty}c_n(x)^n$, and let $R>0$ (or $R=\infty$) be the radius of convergence. And let $f(x)=\sum_{n=0}^{\infty}c_n(x)^n$ be the function defined on $(-R,R)$. Then:
	- (a.) The function $f$ is continuous on $(-R,R)$. (if the series converges at $R$ or $-R$, then $f$ is continuous at $R$ or $-R$, respectively.)
	- (b.) for all $0<r<R$, the function $f$ is integrable on $[-r,r]$. And for all $x\in(-R,R)$, we have $\int_{0}^{x}f(t)dt=\sum_{n=0}^{\infty}\frac{c_n}{n+1}x^{n+1}$.
	- (c.) The function $f$ is continuously differentiable on $(-R,R)$, and for all $x\in(-R,R)$, we have $f'(x)=\sum_{n=0}^{\infty}c_n(n+1)x^n=\sum_{n=1}^{\infty}nc_nx^{n-1}$.
	- The power series in (b.) and (c.) have the same radius of convergence $R$ as the original power series.


### Prop. Censor's Lecture

- Given a power series $\sum_{n=0}^{\infty}c_n(x)^n$. 
	- If the series converges for $x=x_0$, then:
		- the series converges absolutely for all $x$ such that $|x|<|x_0|$.
		- The series converges uniformly on every closed interval $[-r,r]$ where $0<r<|x_0|$.
	- (D'Alambert) $R=\displaystyle\lim_{n\to\infty}\left|\frac{a_{n}}{a_{n+1}}\right|$ is the radius of convergence. given the limit exists.
	- (Cauchy-Hadamard) $R=\displaystyle\frac{1}{\displaystyle\lim{n\to\infty}\sqrt[n]{|a_n|}}$ is the radius of convergence. given the limit exists.
	- (Cauchy-Hadamard, Stonger Version) $R=\displaystyle\frac{1}{\displaystyle\limsup{n\to\infty}\sqrt[n]{|a_n|}}$ is the radius of convergence. (the limit always exists)
	- If the limit is $\infty$, then $R=0$, and if the limit is $0$, then $R=\infty$.
	- The series converges in $R$ (or $-R$) if and only if the series converges uniformly on $[0,R]$ (or $[-R,0]$, respectively).

- Definition: Given a function $f$ defined on $[-R,R]$. If there exists a power series $\sum_{n=0}^{\infty}c_n(x)^n$ such that $f(x)=\sum_{n=0}^{\infty}c_n(x)^n$ for all $x\in[-R,R]$, then we say that $f$ can be represented by a power series on $[-R,R]$.
	- If $f$ can be represented by a power series on $[-R,R]$, then: 
		- The power series is unique, and the coefficients given by $c_n=\frac{f^{(n)}(0)}{n!}$.
		- The function $f$ differentiable infinitely many times on $(-R,R)$.
- If $f$ differentiable infinitely many times on $(-R,R)$, then $f$ can be represented by a power series on $[-R,R]$ if and only if for all $x\in(-R,R)$, we have $\displaystyle\lim_{n\to\infty}R_n(x)=0$ where $R_n(x)=\frac{f^{(n+1)}(x)}{(n+1)!}$ is the remainder of the $n$-th Taylor polynomial of $f$ at $x$. 


- If $f$ differentiable infinitely many times on $(-R,R)$, and there exists $M$ such that $|f^{(n)}(x)|\leq M$ for all $x\in(-R,R)$ and $n\in\mathbb{N}$, then $f$ can be represented by a power series on $[-R,R]$.

- Given a power series $f(x)=\sum_{n=0}^{\infty}a_n(x)^n$ on $[-R,R]$ that converges to $f$ on $[-R,R]$. Then:
	- For all $x\in(-R,R)$, we have $f'(x)=\sum_{n=1}^{\infty}a_nn(x)^{n-1}$. And radius of convergence of $f'$ is $R$ as well. (it's possible that the series of $f$ converges in $\pm R$, but the series of $f'$ converges does not.)
	- For all $x\in(-R,R)$, we have $\int_{0}^{x}f(t)dt=\sum_{n=0}^{\infty}\frac{a_n}{n+1}x^{n+1}$. And radius of convergence of $\int_{0}^{x}f(t)dt$ is $R$ as well. (it's possible that the series of $f$ converges in $\pm R$, but the series of $\int_{0}^{x}f(t)dt$ converges does not.)

- Given power series $f(x)=\sum_{n=0}^{\infty}a_n(x)^n$ and $g(x)=\sum_{n=0}^{\infty}b_n(x)^n$ that converges to $f$ and $g$, respectively. Then:
	- (a.) $\sum c a_n x^n$ converges to $cf(x)$.
	- (b.) $\sum (a_n+b_n)x^n$ converges to $f(x)+g(x)$.
	- (c.) $c_n=\sum_{k=0}^{n}a_kb_{n-k}$, then $\sum c_nx^n$ converges to $f(x)g(x)$. (Cauchy product)
	- (d.) #todo composition of power series



### Behavior of Power Series at Points $|x|=R$



##### Taylor Series

- The **Taylor series** of a function $f$ at a point $a$ is the power series $\sum_{n=0}^{\infty}\frac{f^{(n)}(a)}{n!}(x-a)^n$.





