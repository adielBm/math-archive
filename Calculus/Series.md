-  An **(infinite) series** is an expression that can be written in the form $\displaystyle\sum _{n=1}^{\infty}a_n=a_{1}+a_{2}+\dots+ a_{n}+\dots$ where $(a_{n})$ is a sequence

	- The numbers $a_{1},a_{2},\dots$ are called the **terms** of the series. The number $a_n$ is called the $n$-th **term** of the series.
	- The sequence $(s_n)$ defined by $s_n=\sum_{k=1}^{n}a_k$ is called the **sequence of partial sums** of the series. The number $s_n$ is called the **$n$-th partial sum** of the series.
	- If $(s_n)$ converges to $L$, we say that the series **converges** and that its **sum** is $L$ and write $$a_1+a_2+a_3+\cdots=\sum_{n=1}^{\infty}a_n=\lim_{ n \to \infty }\sum _{k=1}^{n}a_k=L$$
	- If the sequence of partial sums $(s_n)$ diverges, then we say that the series **diverges**.  
		- If $\displaystyle\lim_{n\to\infty}s_n=\infty$, then we say that the series **diverges to infinity**. And denote its sum by $\sum_{n=1}^{\infty}a_n=\infty$. 
		- If $\displaystyle\lim_{n\to\infty}s_n=-\infty$, then we say that the series **diverges to negative infinity**. And denote its sum by $\sum_{n=1}^{\infty}a_n=-\infty$.

# Well-known Series

- A **telescoping series** is a series of the form $\displaystyle\sum_{n=1}^{\infty}(b_n-b_{n+1})$.
- A **telescoping sum** is a sum of the form $\displaystyle\sum_{n=1}^{N}(b_n-b_{n+1})=b_1-b_{N+1}$.

- A **geomorphic series** is a series of the form $\sum_{n=0}^{\infty}ar^n$ where $a\neq0$ and the **common ratio** $r$ are constants.
	- Finite series
		-  ${\sum _{k=1}^{n}ar^{k-1}={\frac {a(1-r^{n})}{1-r}}}$
	- Infinite series
		- if $|r|<1$, $\sum_{n=0}^{\infty}ar^n=\frac{a}{1-r}$.
		- if $|r|\geq1$, $\sum_{n=0}^{\infty}ar^n$ diverges.
			- if $r=1$, $\sum_{n=0}^{\infty}ar^n$ diverges to $\infty$ if $a>0$ (or $-\infty$ if $a<0$).

- A series of the form $\sum_{n=1}^{\infty}\frac{1}{n^p}$ is called a **p-series**. 
	- (e5.8) The p-series converges if $p>1$ and diverges if $p\leq1$.
	- When $p=1$, the series is called the **harmonic series** $\sum_{n=1}^{\infty}\frac{1}{n}$, which diverges.

- The **alternating harmonic series** is the series $\sum_{n=1}^{\infty}\frac{(-1)^{n+1}}{n}=\ln 2$.



# Arithmetic

- Additivity (5.9) - If $\sum_{k=1}^{\infty}a_k$ and $\sum_{k=1}^{\infty}b_k$ converge, then $\sum_{k=1}^{\infty}(a_k\pm b_k)$ converges and $\sum_{k=1}^{\infty}(a_k\pm b_k)=\sum_{k=1}^{\infty}a_k\pm\sum_{k=1}^{\infty}b_k$.
- (5.10) If $c\neq0$, then $\sum_{k=1}^{\infty}a_k$ converges if and only if $\sum_{k=1}^{\infty}ca_k$ converges and $\sum_{k=1}^{\infty}ca_k=c\sum_{k=1}^{\infty}a_k$.
- If $\sum_{k=1}^{\infty}a_k$ converges, then $\sum_{k=1}^{\infty}ca_k$ converges and $\sum_{k=1}^{\infty}ca_k=c\sum_{k=1}^{\infty}a_k$.
- (q5.12) If $\sum_{k=1}^{\infty}a_k=\infty$, and $c>0$, then $\sum_{k=1}^{\infty}ca_k=\infty$.  

- Convergence or divergence is unaffected by deleting a finite number of terms from a series; in particular, for any positive integer $K$, the series $\sum_{k=1}^{\infty}a_k$ converges if and only if the series $\sum_{k=K}^{\infty}a_k$ converges.



# Convergence tests

- Strategy for Series https://eddieguo.ca/assets/downloads/notes/math101.pdf


- (q5.16) Given a convergent series $\sum_{k=1}^{\infty}a_k$, then $\displaystyle\lim_{n\to\infty}{\sum_{k=n+1}^{\infty}a_k}=0$.

- (5.4) Cauchy's convergence test - The series $\sum_{k=1}^{\infty}a_k$ converges if and only if $\forall\varepsilon>0\exists N\in\mathbb{N}:\forall n\geq N\forall p\in \mathbb{N},\left|\sum_{k=n+1}^{n+p}a_k\right|<\varepsilon$.
- (5.5) If $\sum_{n=1}^{\infty}a_n$ converges, then $\displaystyle\lim_{n\to\infty}a_n=0$.
- (The Divergence Test) If $\displaystyle\lim_{n\to\infty}a_n\neq0$, then $\sum_{n=1}^{\infty}a_n$ diverges.
- (5.6) If $\sum_{n=1}^{\infty}\left|a_n\right|$ converges, then $\sum_{n=1}^{\infty}a_n$ converges.
- The Integral Test - Let $\sum_{k=1}^{\infty}a_k$ be a series of positive terms. If $f$ is a continuous, positive, and decreasing function on $[a, \infty)$ such that $f(k)=a_k$ for all $k\geq a$, then the series $\displaystyle\sum_{k=1}^{\infty}a_k$ and the improper integral $\displaystyle\int_{a}^{\infty}f(x)dx$ either both converge or both diverge.
- (5.11) #todo 
- (5.12) Let $k$ be a natural number. The series $\sum_{n=1}^{\infty}a_n$ converges if and only if the series $\sum_{n=1}^{\infty}a_{n+k}$ converges.
	- In which case, $\sum_{n=1}^{\infty}a_n=(a_1+a_2+\cdots+a_k)+\sum_{n=1}^{\infty}a_{n+k}$.
	- (q5.14) Let $m$ be a natural number. $\sum_{k=1}^{\infty}a_k=\infty$ if and only if $\sum_{k=m}^{\infty}a_{k}=\infty$.


- (5.13) If $a_n\geq0$ for all $n$, then the sequence of partial sums $(s_n)$ is increasing.
	- The series $\sum_{n=1}^{\infty}a_n$ converges if and only if the sequence of partial sums $(s_n)$ is bounded above.
	- The series $\sum_{n=1}^{\infty}a_n$ diverges to infinity if and only if the sequence of partial sums $(s_n)$ is unbounded. 


### Comparison test

- The Comparison Test (5.14, "first") - Given series $\sum a_n$ and $\sum b_n$. If $0\leq a_n\leq b_n$ for all $n>N$, then
	- If $\sum b_n$ converges, then $\sum a_n$ converges.
	- If $\sum a_n$ diverges, then $\sum b_n$ diverges.	(they both diverge to infinity)

### Limit Comparison Test

- The Limit Comparison Test (5.15, "second") - Given series $\sum a_n$ and $\sum b_n$. If $\displaystyle\lim_{n\to\infty}\frac{a_n}{b_n}=c$, where $c$ is a positive real number, then
	- The series $\sum a_n$ converges, if and only if the series $\sum b_n$ converges.
- (q5.21) Given $a_n\geq0$ and $b_n\geq0$ for all $n>N$. 
	- If $\displaystyle\lim_{n\to\infty}\frac{a_n}{b_n}=0$, and $\sum b_n$ converges, then $\sum a_n$ converges.
	- If $\displaystyle\lim_{n\to\infty}\frac{a_n}{b_n}=\infty$, and $\sum b_n$ diverges, then $\sum a_n$ diverges.

### Root test (Cauchy)

- (5.16) Root test (Cauchy)
	- (a.) If there exists $q<1$ such that $\sqrt[n]{|a_n|}\leq q$ for almost all $n$, then the series $\sum a_n$ converges absolutely. 
	- (b.) If $\sqrt[n]{|a_n|}\geq 1$ for infinitely many $n$, then the series $\sum a_n$ diverges.

- (5.16*) Given $c=\displaystyle\limsup_{n\to\infty}\sqrt[n]{|a_n|}$. or ($c=\displaystyle\lim_{n\to\infty}\sqrt[n]{|a_n|}$ exists (5.16**))
	- If $c<1$, then the series $\sum a_n$ converges absolutely.
	- If $c>1$, then the series $\sum a_n$ diverges.
	- If $c=1$, then the test is inconclusive.

### Ratio test (d'Alembert)

- Ratio test (d'Alembert) (given $a_n\neq0$ for all $n$)
	- (5.17) 
		- (a.) If there exists $q<1$ such that $\left|\frac{a_{n+1}}{a_n}\right|\leq q$ for almost all $n$, then the series $\sum a_n$ converges absolutely.
		- (b.) If $\left|\frac{a_{n+1}}{a_n}\right|\geq 1$ for almost all $n$, then the series $\sum a_n$ diverges.
	- (5.17**) Given $c=\displaystyle\lim{n\to\infty}\left|\frac{a_{n+1}}{a_n}\right|$.
		- If $c<1$, then the series $\sum a_n$ converges absolutely.
		- If $c>1$, then the series $\sum a_n$ diverges.
		- If $c=1$, then the test is inconclusive.
	(q5.26) If there exists $q<1$ such that $\left|\frac{a_{n+1}}{a_n}\right|\leq q<1$ for almost all $n$, then there exists $q\leq q'<1$ such that $\sqrt[n]{|a_n|}\leq q'$ for almost all $n$.

### Cauchy condensation test

- (5.18) Cauchy condensation test - Let $(a_n)$ be a [[Calculus/Sequences/Monotonicity|decreasing]] sequence of nonnegative terms. The series $\sum_{n=1}^{\infty}a_n$ converges if and only if the series $\sum_{n=1}^{\infty}2^na_{2^n}$ converges.

# Convergence Absolutely

- (d5.7) A series $\sum_{n=1}^{\infty}a_n$ is said to **converge absolutely** if the series of absolute values $\sum_{n=1}^{\infty}|a_n|$ converges.
- (d5.8) A series $\sum_{n=1}^{\infty}a_n$ is said to **converge conditionally** if it converges but does not converge absolutely.



# Exmaples

- $\displaystyle\sin x=\sum_{n=0}^{\infty}\frac{(-1)^n}{(2n+1)!}x^{2n+1}$ 
- $\displaystyle\cos x=\sum_{n=0}^{\infty}\frac{(-1)^n}{(2n)!}x^{2n}$ 
- $\displaystyle e^x=\sum_{n=0}^{\infty}\frac{1}{n!}x^n$
- $\displaystyle e^{-x}\sum_{n=0}^{\infty}\frac{(-1)^n}{n!}x^n$
- $\displaystyle\ln(1+x)=\sum_{n=1}^{\infty}\frac{(-1)^{n+1}}{n}x^{n}$
- $\displaystyle\ln(1-x)=-\sum_{n=1}^{\infty}\frac{1}{n}x^{n}$









