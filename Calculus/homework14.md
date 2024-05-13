


# Definitions 

Let $f$ be a [[Derivative#Higher-order derivatives|n-times differentiable]] function, the polynomial $$\displaystyle P_{n}(x)=\sum _{k=0}^{n}{\frac {f^{(k)}(a)}{k!}}(x-a)^{k}$$ is called the $n$th order **Taylor polynomial** of $f$ centered at $a$.
- When $a=0$, the polynomial $$P_{n}(x)=\sum _{n=0}^{n}{\frac {f^{(k)}(0)}{k!}}x^{k}$$ is called also the **Maclaurin polynomial** of $f$
- The function $R_{n}(x)=f(x)-P_{n}(x)$ is called the n-th **remainder** of $f$ at $a$
	- (פיתוח טיילור) $f(x)=P_{n}(x)+R_{n}(x)$ 
- Properties
	- $P_{n}^{(m)}(a)=f^{(m)}(a)$ (for all $m=0,\dots,n$)
	- (q4.11) Let $f(x)=x^k$ for $k\in\mathbb{N}$, and $P_{n}(x)$ Maclaurin polynomial of $f$, and $R_{n}(x)$ the reminder, then
		- for all $k>n$, $f(x)=R_{n}(x)$
		- for all $k\leq n$, $f(x)=P_{n}(x)$



# Exercise 1

- Show that $1+\frac{x-1}{2}-\frac{(x-1)^2}{8}$ approachs $\sqrt{x}$ in $[\frac{1}{2},\frac{3}{2}]$ in approximation of one digit after the decimal point. (i.e. in apporx of 0.5 * 10^(-1)).


answer:

We have to show that $\displaystyle\left|\sqrt{x}-(1+\frac{x-1}{2}-\frac{(x-1)^2}{8})\right|< 0.5 \cdot 10^{-1}=\frac{1}{20}$ for all $x\in[\frac{1}{2},\frac{3}{2}]$.


The taylor polynomial of $\sqrt{x}$ is at $a$ of order 2 is:

$$P_{2}( x) =\sum _{k=0}^{2}\frac{\sqrt{a}^{( k)}}{k!}( x-a)^{k} =\sqrt{a}^{( 0)} +\frac{1}{2\sqrt{a}}( x-a) \ -\frac{1}{8a^{3/2}}( x-a){^{2}}$$

where $a=1$ then: 

$$P_{2}(x)=1+\frac{x-1}{2}-\frac{( x-1)^{2}}{8}$$


Lagrange’s Form is given by:

$$\displaystyle R_{n}(x)=\frac{f^{(n+1)}(c)}{(n+1)!}(x-a)^{n+1}$$

so in our case,  

$$R_{2}(x)=\frac{f^{(3)}(c)}{3!}(x-1)^{3}$$

where $c\in(1,x)$ or $c\in(x,1)$, and $\vert x - 1 \vert \leq \frac{1}{2}$.

now the third derivative of $\sqrt{x}$ is:

$$f^{(3)}(x)=\frac{3}{8}x^{-5/2}\leq f^{(3)}(\frac{1}{2})=\frac{3}{8}2^{5/2}=\frac{3\sqrt{2}}{2}$$ 

(f is decreasing)

consequently,



$$
\left|\sqrt{x}-(1+\frac{x-1}{2}-\frac{(x-1)^2}{8})\right|=\left|R_{2}(x)\right|=

\\

=\left|\frac{f^{(3)}(c)}{3!}(x-1)^{3}\right|\leq \frac{3\sqrt{2}}{2 \cdot !3}\cdot \left(\frac{1}{2}\right)^{3}=\frac{3\sqrt{2}}{96}=\frac{\sqrt{2}}{32}<\frac{1}{20}$$



a **similar** solution can be found in the book "Calculus" by Michael Spivak, page 233, problem 4-11.



# Exercise 2

Given $f(x)=xe^{x}$.


- (A.) Find the Taylor polynomial of $f$ of order n centered at $a=0$.
- (B.) Find the Maclaurin polynomial of $f$ of order n. And prove that for all x the remainder is approaching 0 as $n\to\infty$.
	- Remark: The point c of lagrange's form is dependent on n.
- (C.) Calculate f(1/3) with an error of at most 0.5 * 10^(-2).

## Answer for A

The $n$th order Taylor polynomial of $f$ centered at $x=a$ is:

$$P_{n}(x)=\sum _{k=0}^{n}{\frac {f^{(k)}(a)}{k!}}(x-a)^{k}$$

where $f(x)=xe^{x}$, then:

$$f^{(k)}(x)=\begin{cases}
xe^{x} & k=0\\
e^{x}+xe^{x} & k=1\\
2e^{x}+xe^{x} & k=2\\
3e^{x}+xe^{x} & k=3\\
\vdots & \vdots\\
ke^{x}+xe^{x} & k=k
\end{cases}$$

then 

$$P_{n}(x)=\sum _{k=0}^{n}{\frac {f^{(k)}(a)}{k!}}(x-a)^{k}=ae^{a}+({e^a + ae^a}){(x-a)}+\dots+\frac{n e^a + a e^a}{n!}(x-a)^{n}$$

## Answer for B

The Maclaurin polynomial of $f(x)=xe^{x}$ of order $n$ is:

$$P_{n}(x)=\sum _{k=0}^{n}{\frac{k}{k!}}x^{k}=\sum _{k=0}^{n}{\frac{1}{(k-1)!}}x^{k}$$

Now we have to show that for all $x$, the limit $\displaystyle\lim_{n\to\infty}R_{n}(x)=\lim_{n\to\infty}{(xe^{x}-P_{n}(x))}=0$.


The remainder of $f$ at $a$ is:

$$R_{n}(x)=\frac{f^{(n+1)}(c)}{(n+1)!}(x)^{n+1}$$

where $\vert c \vert < \vert x \vert$

then

$$\vert R_{n}(x) \vert = \frac{\vert f^{(n+1)}(c) \vert}{(n+1)!}\vert x \vert^{n+1}= \frac{\vert (n+1)e^{c}+ce^{c} \vert}{(n+1)!}\vert x \vert^{n+1}$$