
- Given a sequence of numbers $(a_{n})$, an expression of the form $a_1+a_2+a_3+\cdots+a_n$ is called a **series**.
- The number $a_n$ is called the $n$-th **term** of the series.
- The sequence $(s_n)$ defined by $s_n=\sum_{k=1}^{n}a_k$ is called the **sequence of partial sums** of the series.
- The number $s_n$ is called the **$n$-th partial sum** of the series.
- If the sequence of partial sums $(s_n)$ converges to a number $L$, then we say that the series **converges** and that its **sum** is $L$ and write $$a_1+a_2+a_3+\cdots=\sum_{n=1}^{\infty}a_n=\lim_{ n \to \infty }s_{n}= L.$$
- If the sequence of partial sums $(s_n)$ diverges, then we say that the series **diverges**.
  - If $\displaystyle\lim_{n\to\infty}s_n=\infty$, then we say that the series **diverges to infinity**. And denote it by $\displaystyle\sum_{n=1}^{\infty}a_n=\infty$.
  - If $\displaystyle\lim_{n\to\infty}s_n=-\infty$, then we say that the series **diverges to negative infinity**. And denote it by $\displaystyle\sum_{n=1}^{\infty}a_n=-\infty$.
  - If a series diverges to infinity (or $-\infty$), then we say that its **sum** is $\infty$ (or $-\infty$).



- If the series $\sum_{n=1}^{\infty}a_n$ converges, then $\displaystyle\lim_{n\to\infty}a_n=0$.
- Test for divergence: If $\displaystyle\lim_{n\to\infty}a_n\neq0$, then the series $\sum_{n=1}^{\infty}a_n$ diverges.


- A **telescoping series** is a series of the form $\displaystyle\sum_{n=1}^{\infty}(b_n-b_{n+1})$.
- A **telescoping sum** is a sum of the form $\displaystyle\sum_{n=1}^{N}(b_n-b_{n+1})=b_1-b_{N+1}$.



- A **geomorphic series** is a series of the form $\sum_{n=0}^{\infty}ar^n$ where $a\neq0$ and the **common ratio** $r$ are constants.
	- Finite series
		-  ${\sum _{k=1}^{n}ar^{k-1}={\frac {a(1-r^{n})}{1-r}}}$
	- Infinite series
		- if $|r|<1$, $\sum_{n=0}^{\infty}ar^n=\frac{a}{1-r}$.
		- if $|r|\geq1$, $\sum_{n=0}^{\infty}ar^n$ diverges.
			- if $r=1$, $\sum_{n=0}^{\infty}ar^n$ diverges to $\infty$ if $a>0$ (or $-\infty$ if $a<0$).
- The **harmonic series** is the series $\sum_{n=1}^{\infty}\frac{1}{n}$. The harmonic series diverges.
- The **alternating harmonic series** is the series $\sum_{n=1}^{\infty}\frac{(-1)^{n+1}}{n}=\ln 2$.

	

- Strategy for Series https://eddieguo.ca/assets/downloads/notes/math101.pdf



# Tests

- (5.4) Cauchy's convergence test - The series $\sum_{k=1}^{\infty}a_k$ converges if and only if $\forall\varepsilon>0\exists N\in\mathbb{N}:\forall n\geq N\forall p\in \mathbb{N},\left|\sum_{k=n+1}^{n+p}a_k\right|<\varepsilon$.
- (5.5) If $\sum_{n=1}^{\infty}a_n$ converges, then $\lim_{n\to\infty}a_n=0$.
- (The Divergence Test) If $\lim_{n\to\infty}a_n\neq0$, then $\sum_{n=1}^{\infty}a_n$ diverges.
- (5.6) If $\sum_{n=1}^{\infty}\left|a_n\right|$ converges, then $\sum_{n=1}^{\infty}a_n$ converges.
- The Integral Test - Let $\sum_{k=1}^{\infty}a_k$ be a series of positive terms. If $f$ is a continuous, positive, and decreasing function on $[a, \infty)$ such that $f(k)=a_k$ for all $k\geq a$, then the series $\displaystyle\sum_{k=1}^{\infty}a_k$ and the improper integral $\displaystyle\int_{a}^{\infty}f(x)dx$ either both converge or both diverge.




# Definitions

- (d5.7) A series $\sum_{n=1}^{\infty}a_n$ is said to **converge absolutely** if the series of absolute values $\sum_{n=1}^{\infty}|a_n|$ converges.
- (d5.8) A series $\sum_{n=1}^{\infty}a_n$ is said to **converge conditionally** if it converges but does not converge absolutely.

# Arithmetic

- Additivity (5.9) - If $\sum_{k=1}^{\infty}a_k$ and $\sum_{k=1}^{\infty}b_k$ converge, then $\sum_{k=1}^{\infty}(a_k\pm b_k)$ converges and $\sum_{k=1}^{\infty}(a_k\pm b_k)=\sum_{k=1}^{\infty}a_k\pm\sum_{k=1}^{\infty}b_k$.
- (5.10) If $c\neq0$, then $\sum_{k=1}^{\infty}a_k$ converges if and only if $\sum_{k=1}^{\infty}ca_k$ converges and $\sum_{k=1}^{\infty}ca_k=c\sum_{k=1}^{\infty}a_k$.
- If $\sum_{k=1}^{\infty}a_k$ converges, then $\sum_{k=1}^{\infty}ca_k$ converges and $\sum_{k=1}^{\infty}ca_k=c\sum_{k=1}^{\infty}a_k$.
- (q5.12) If $\sum_{k=1}^{\infty}a_k=\infty$, and $c>0$, then $\sum_{k=1}^{\infty}ca_k=\infty$.  

- Convergence or divergence is unaffected by deleting a finite number of terms from a series; in particular, for any positive integer $K$, the series $\sum_{k=1}^{\infty}a_k$ converges if and only if the series $\sum_{k=K}^{\infty}a_k$ converges.



# Exmaples

- $\displaystyle\sin x=\sum_{n=0}^{\infty}\frac{(-1)^n}{(2n+1)!}x^{2n+1}$ 
- $\displaystyle\cos x=\sum_{n=0}^{\infty}\frac{(-1)^n}{(2n)!}x^{2n}$ 
- $\displaystyle e^x=\sum_{n=0}^{\infty}\frac{1}{n!}x^n$
- $\displaystyle e^{-x}\sum_{n=0}^{\infty}\frac{(-1)^n}{n!}x^n$
- $\displaystyle\ln(1+x)=\sum_{n=1}^{\infty}\frac{(-1)^{n+1}}{n}x^{n}$
- $\displaystyle\ln(1-x)=-\sum_{n=1}^{\infty}\frac{1}{n}x^{n}$









