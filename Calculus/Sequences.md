
- (2.17) A sequence obtained by changing a finite number of terms they has the same limit 

- (d2.8) $N_{\varepsilon}(a):=\set{x\in\mathbb{R}: |x-a|<\varepsilon}$ where $\varepsilon>0$ and a is real number is $\varepsilon$-**neighborhood** of the real number $a$


# Bound

- (q2.19a,b,f) The sum/difference/product of two bounded sequences is a sequence bounded
- (q2.19d) The sum of bounded sequence and unbounded sequence and is unbounded sequence


- (2.16) every convergent sequence is bounded

# Monotonicity

**definitions**
- monotone sequence (either increaseing or decreaseing)
	- monotonically increasing: $a_{n}+1≥a_n$ for all $n\in\mathbb{N}$
		- strictly monotonically increasing: $a_{n}+1>a_n$ for all $n\in\mathbb{N}$
	- monotonically decreasing: $a_{n}+1\leq a_n$ for all $n\in\mathbb{N}$
		- strictly monotonically decreasing: $a_{n}+1<a_n$ for all $n\in\mathbb{N}$

**Theorems**
- Monotone convergence theorem
	- (3.16) if $(a_{n})$ is a **monotone** and **bounded** sequence, then it's convergent
		-  if $(a_{n})$ is **increasing** bounded, then $\lim_{ n \to \infty }(a_{n})=\sup(a_{n})$
		-  if $(a_{n})$ is **decreasing** bounded, then $\lim_{ n \to \infty }(a_{n})=\inf(a_{n})$
	- (3.17) if $(a_{n})$ is a **monotone** and **not-bounded** sequence, then
		-  if $(a_{n})$ is **increasing**, then $\lim_{ n \to \infty }(a_{n})=\infty$
		-  if $(a_{n})$ is **decreasing**, then $\lim_{ n \to \infty }(a_{n})=-\infty$

# Convergence & Limit

- $\lim_{ n \to \infty }{a_{n}}=L$
- The sequence $(a_n)$ is said to **converge to** or **tend to** the limit $L$.
- For each real number $\varepsilon >0$, there exists a natural number $N$ such that, for every natural number $n>N$, we have ${\displaystyle |a_{n}-L|<\varepsilon }$
- $\forall \varepsilon > 0 \left(\exists N \in \mathbb{N} \left(\forall n \in\mathbb{N}\left(n \geq N \implies |a_n - L| < \varepsilon \right)\right)\right)$

- Arithmetic (2.28)
	- $(a_{n})_{n=1}^{\infty}$ and $(b_{n})_{n=1}^{\infty}$ are convergent
		- $(c\cdot a_{n})_{n=1}^{\infty}$ is convergent, and $\lim_{ n \to \infty }({ca_{n})}=c\cdot\lim_{ n \to \infty }{a_{n}}$
		- $\lim_{n\to\infty} (a_n \pm b_n) =  \lim_{n\to\infty} a_n \pm \lim_{n\to\infty} b_n$
		- $\lim_{n\to\infty} (a_n \cdot b_n) =  \left(\lim_{n\to\infty} a_n \right)\cdot \left( \lim_{n\to\infty} b_n \right)$
		- $\lim_{n\to\infty} \left(\frac{a_n}{b_n}\right) = \frac{\lim\limits_{n\to\infty} a_n}{\lim\limits_{n\to\infty} b_n}$ (provided $\lim_{n\to\infty} b_n \ne 0$)
		- $\lim_{n\to\infty} a_n^k =  \left( \lim_{n\to\infty} a_n \right)^k$


**theorems**

- (2.29) **Shift Rule** Let $N$ be a natural number. Let $(a_{n})$ be a sequence. Then $a_{n} → a$ if and only if the *shifted* sequence $a_{N+n}→a$.
- Let $(a_n)$ and $(b_n)$ be two convergent sequences:
	- (2.30) if $\lim_{n \to \infty} a_n <\lim_{n \to \infty} b_n$ then, for almost all $n$, we have $a_n < b_n$
	- (2.31) if $a_n \leq b_n$ for each $n$, then $\lim_{n \to \infty} a_n \leq\lim_{n \to \infty} b_n$
- (2.32) **Squeeze theorem**  - let $(a_n)$, $(b_n)$, and $(c_n)$ sequences, where (1.) $a_{n}\leq b_{n}\leq c_{n}$ for almost all $n$. (2.)   $(a_n)$, and $(c_n)$ are convergent. (3.) $\lim_{n \to \infty} a_n =\lim_{n \to \infty} c_n=L$. **then**, $\lim_{n \to \infty} b_n=L$
- (2.33) $-1<a<1\implies\lim_{n \to \infty}a^n=0$
- (2.34) $a>0\implies\lim_{n \to \infty}\sqrt[n]{ a }=1$
- $\lim_{n\rightarrow\infty}\sqrt[n]n=1$
- (q2.29) let $a_{1},\dots ,a_{k}\geq 0$, then $\lim_{n\to\infty} \sqrt[n]{\sum_{i=1}^k a_{i}^n}=\max\set{a_{1},\dots ,a_{k}}$

- #todo For any continuous function $f$, if $\lim _{n\to \infty }a_{n}$ exists, then $\lim _{n\to \infty }f\left(a_{n}\right)$ exists too.


## Null Sequence 

definitions 
- (d2.21) $(a_{n})$ is null sequence 
- $\lim_{n \mathop \to \infty} {a}_n=0$
- (q2.20a) $(|a_{n}|)$ is null sequence

properties of null sequence $(a_{n})$
- $(a_{n})$ is bounded sequence


- (2.22) product of **null** and **bounded** sequences is **null** sequence



## Infinite limits

**equivalent definitions**
- $(a_{n})$ is said to **tend to infinity**, written $a_{n}\to \infty$, or $\lim _{n\to \infty }a_{n}=\infty$
- For every real number $K$, there is a natural number $N$ such that for every natural number $n\geq N$, we have  $a_{n}>K$; that is, the sequence terms are eventually larger than any fixed $K$.
- $\forall K\in \mathbb {R} \left(\exists N\in \mathbb {N} \left(\forall n\in \mathbb {N} \left(n\geq N\implies a_{n}>K\right)\right)\right).$
- (2.39) $\lim_{n\to\infty}(-a_{n})=-\infty$

**properties**
- (2.40) If a sequence tends to infinity or minus infinity, then it is unbounded.
- (2.41) If a sequence tends to infinity or minus infinity, then it is divergent.



theorems:
- (2.44) #todo like 2.29 but for infinite limit 
-  **Squeeze Theorem** for infinite limit 
	- (2.45) if $a_{n}\to \infty$ and $b_{n}\geq a_{n}$ for almost all $n$, then $b_{n}\to \infty$
	- (q2.40) if $a_{n}\to -\infty$ and $b_{n}\leq a_{n}$ for almost all $n$, then $b_{n}\to -\infty$

- (2.43, q2.39) **arithmetics of infinite limits**
	- ${a_{n}\to \infty}\land{b_{n}\to \infty}\implies a_{n}+b_{n}\to \infty$
	- ${a_{n}\to \infty}\land{\lim_{ n \to \infty }b_{n}\in \mathbb{R}}\implies a_{n}+b_{n}\to \infty$
	- ${a_{n}\to \infty}\land{b_{n}\to \infty}\implies a_{n}b_{n}\to \infty$
	- ${a_{n}\to \infty}\land{\lim_{ n \to \infty }b_{n}>0}\implies a_{n}b_{n}\to \infty$
	- ${a_{n}\to \infty}\implies 1/a_{n}\to0$
	- (q2.57a) ${|a_{n}|\to \infty}\implies 1/a_{n}\to0$
	- ${a_{n}\to 0}\land{a_{n}>0} \implies 1/a_{n}\to{\infty}$
	- ${a_{n}\to \infty}\land{b_{n}\to (-\infty)} \implies a_{n}b_{n}\to{(-\infty)}$
	- ${a_{n}\to (-\infty)}\land{b_{n}\to (-\infty)} \implies a_{n}b_{n}\to{\infty}\land  a_{n}+b_{n}\to{(-\infty)}$
	- ${a_{n}\to 0}\land{a_{n}<0} \implies 1/a_{n}\to{(-\infty)}$
	- ${a_{n}\to \infty}$ and ${b_{n}}$ is bounded $\implies a_{n}+b_{n}\to \infty$

# Order

- $(a_{n})$ and $(b_{n})$ are **positive (!!!)**
	- definitions
		- $a_{n}=O(b_{n})\iff \exists{c>0}:{a_{n}\leq cb_{n}}$ (for all $n$) $\iff$ $(a_{n}/b_{n})$ is bounded (q2.44a)
		- $a_{n}=o(b_{n})\iff {\lim_{ n \to \infty }(a_{n}/b_{n})=0}\iff{\lim_{ n \to \infty }(b_{n}/a_{n})=\infty}$
	- theorems
		- (q2.45a) $\lim_{ n \to \infty }(a_{n}/b_{n})=c\in{\mathbb{R}}\implies a_{n}=O(b_{n})$
		- (q2.44b) $a_{n}=o(b_{n})\implies a_{n}=O(b_{n})$
		- (q2.44c) $a_{n}=O(1)\iff{(a_{n})}$ is bounded
		- (q2.45c) **Transitivity** - $a_{n}=o(b_{n})\land{b_{n}=o(c_{n})}\implies a_{n}=o(c_{n})$
		- (2.49) for each $k$ natural, and $r>1$ real: $\lim_{ n \to \infty }\left( \frac{n^k}{r^n} \right)=0$ (*i.e.* $n^k=o(r^n)$, 2.50) 

# Ratio test

- $(a_{n})$ is sequence (all are nonzero)

- if $\lim _{n\to \infty }\left|{\frac {a_{n+1}}{a_{n}}}\right|<1$ then $\lim_{ n \to \infty }(a_{n})=0$
	- if $\lim _{n\to \infty }{\frac {a_{n+1}}{a_{n}}}>1$ (or $=\infty$) and $a_{n}>0$, then $\lim_{ n \to \infty }(a_{n})=\infty$
	 

#  Mean Sequences

-  Arithmetic Mean Sequence
	- (2.51) if $b_n=\frac{1}{n}\sum^{n}_{i=1}{a_i}$ then $(b_{n})$ is the **arithmetic mean sequence** of $(a_{n})$
		- $\lim_{ n \to \infty }(a_{n})=L\in\mathbb{R}\implies \lim_{ n \to \infty }(b_{n})=L$
		- $a_{n}\to \infty\implies b_{n}\to \infty$
		- $a_{n}\to -\infty\implies b_{n}\to -\infty$

-  Geometric Mean Sequence
	- (2.52) if $c_n=\sqrt[n]{\prod^{n}_{i=1}{a_i}}$ then $(c_{n})$ is the **geometric mean sequence** of $(a_{n})$
		- #todo 

- (3.22) **Cantor's intersection** theorem (Cantor's Lemma)
	- Let $(I_{n})^{\infty}_{n=1}$ be a sequence of non-empty, closed intervals, $I_{n}=[a_{n},b_{n}]$, satisfying $I_{1}\supseteq I_{2}\supseteq I_{3}\supseteq\dots$ and $\lim_{ n \to \infty }(b_{n}-a_{n})=0$, then, $\bigcap_{n=1}^{\infty}I_{n}=\{ x \}$, and $x=\lim_{ n \to \infty }(a_{n})=\lim_{ n \to \infty }(b_{n})$
	- Let $(a_{n})^{\infty}_{n=1}$ and $(b_{n})^{\infty}_{n=1}$ be two sequence of real numbers that satisfy: $a_{n}\leq a_{n+1} < b_{n+1}\leq b_{n}$ for every $n\in\mathbb{N}$, and $\lim(b_{n}-a_{n})=0$. Then there exists a real number $c$ such that $\lim a_{n}=\lim b_{n}=c$. The number $c$ is the unique real number that satisfies $a_{n} \leq c\leq b_{n}$


# Subsequence

- (d3.24) Let $(a_{n})$ be a sequence of real numbers and let $n_{1}<n_{2}<\dots<n_{k}<\dots$ be a strictly increasing sequence of real numbers. Then the sequence $(a_{n_{k}})$ given by $(a_{n_{1}},a_{n_{2}},\dots,a_{n_{k}},\dots)$ is called **subsequence of** $(a_{n})$

- (3.25) if $(a_{n})$ converges to $x$ (or $\pm \infty$) then every subsequence of $(a_{n})$ is also converges to $x$ (or $\pm \infty$)
- (3.32) **Bolzano–Weierstrass theorem** - Every bounded sequence has a convergent subsequence
- (3.33) Every sequence has a *convergent* (or *tends to infinity*) subsequence
- (q3.48) **Monotone Subsequence Theorem** - Every sequence has a monotonic subsequence

# Subsequential Limit

- (E.D) of subsequential limit  
	- $L\in\mathbb{R}$ is **subsequential limit** of $(a_{n})^{\infty}_{n=1}$ 
	- (d3.26) There exists subsequence $(a_{n_{k}})^{\infty}_{k=1}$ such that $a_{n_{k}}\to L$
	- (3.27) $\forall{ε>0}$ there are infinite $n$ values for which $|a_n-L|<ε$
	- (3.27) $\forall{ε>0},\forall{N\in\mathbb{N}},\exists{n>N},|a_n-L|<ε$
	- (3.27 geometrically) For every neighborhood of $L$ there are infinite terms of $(a_{n})$

- examples:
	- $\set{0,1}$ is the set of subsequential limits of $a_n = \begin{cases} {1}/{n} & \text{if } n \text{ is even} \\ {n}/{(n+1)} & \text{if } n \text{ is odd} \end{cases}$
	- (by 3.25) if convergent sequence $(a_{n})\to{L}$ then $L$ is the only subsequential limit. 
	- (3.34) A bounded sequence is convergent, if and only if, it has exactly one subsequential limit.


- (3.32) **Bolzano–Weierstrass theorem** - Every bounded sequence has a subsequential limit.

# Limit Inferior & Limit Superior
	
- The **limit inferior** of a sequence $(a_{n})$
	- $\displaystyle  {\displaystyle \liminf _{n\to \infty }a_{n}:=\lim _{n\to \infty }\!{\Big (}\inf _{m\geq n}a_{m}{\Big )}}$
- The **limit superior** of a sequence $(a_{n})$
	- $\displaystyle  {\displaystyle \limsup _{n\to \infty }a_{n}:=\lim _{n\to \infty }\!{\Big (}\sup _{m\geq n}a_{m}{\Big )}}$



