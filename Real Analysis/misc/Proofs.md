# Unit 1

## (1.43) Bernoulli's Inequality 
 $$x>-1\implies\forall n \in \mathbb{N},({1 + x})^n \ge 1 + n x$$

| Proof by Induction |  |
| ---- | ---- |
| base case |  |
| $n=1\implies 1+x\geq 1+x$ |  |
| induction step |  |
| $({1 + x})^n \ge 1 + n x$ | induction hypothesis |
| $(1+x )({1 + x})^n \ge(1+x )(1 + n x)$ | multiplying by $(1+x)\geq 0$ (because $x>-1$) |
| $({1 + x})^{n+1} \ge1+x+nx+nx^2$ |  |
| $({1 + x})^{n+1} \ge 1+(n+1)x+nx^2$ |  |
| $(1+x)^{n+1}\geq 1+(n+1)x$ | because $nx^2\geq 0$ |
## (1.47) Existence minimum and maximum of set 

- Let $A = \{x_1, \ldots,x_n\}$ be a **nonempty** finite set of size $n > 0$. Then there exist some $m,M \in A$ such that for all $x \in S$, we have that $m \leq x \leq M$

| Proof by Induction (for maximum) |  |
| ---- | ---- |
| **Base Case** |  |
| For $n=1$, let $A=\{x_1\}$ |  |
| $M=x_1$ | Trivially, $M=x_1$ holds |
| **Induction Step** |  |
| $\exists M:\forall x \in A,\,x\leq M$ | Inductive hypothesis |
| if $x_{n+1}>\max\{ x_{1},\dots,x_{n} \}$ then $M:=x_{n+1}$<br>if $x_{n+1}\leq\max\{ x_{1},\dots,x_{n} \}$ then $M:=\max\{ x_{1},\dots,x_{n} \}$ |  |
# Unit 2
## (2.12) Limit Uniqueness

Let $(a_n)$ be a convergent sequence
$$( \lim_{ n \to \infty } a_{n}=L \land{\lim_{ n \to \infty } a_{n}=M})\implies{L=M}$$

#todo check it!!

| Proof by Contradiction |  |
| ---- | ---- |
| $L\neq M$ | Assume by contradiction |
| $\displaystyle\varepsilon=\frac{\vert L-M\vert}{3}>0$ | because $L\neq M$ |
| $\exists N_{1}:\forall n>N_{1},\vert{a_{n}-L}\vert<\varepsilon$ | because $\displaystyle{\lim_{ n \to \infty } a_{n}=L}$ |
| $\exists N_{2}:\forall n>N_{2},\vert{a_{n}-M}\vert<\varepsilon$ | because $\displaystyle{\lim_{ n \to \infty } a_{n}=M}$ |
| $n:=\max\{ N_{1}, N_{2} \}+1$ |  |
| $n>N_{1},n>N_{2}$ |  |
| $\vert{a_{n}-L}\vert<\varepsilon,\vert{a_{n}-M}\vert<\varepsilon$ |  |
| $\vert{L-M}\vert \leq \vert{a_{n}-L}\vert + \vert{a_{n}-M}\vert$ | Triangle inequality |
| $\vert{L-M}\vert < \varepsilon + \varepsilon$ |  |
| $\vert{L-M}\vert < \frac{\vert L-M\vert}{3} + \frac{\vert L-M\vert}{3}$ | Substituting $\varepsilon$ |
| $\vert{L-M}\vert < \frac{2\vert L-M\vert}{3}$ | Combining like terms |
| $3\vert{L-M}\vert < 2\vert L-M\vert$ | Multiplying both sides by 3 |
| $3<2$ | Dividing by $\vert L-M\vert$ both sides |
| **Contradiction!** |  |
|  |  |

## (2.16) Convergent sequence is Bounded

|  |  |
| ---- | ---- |
| $\displaystyle\lim_{ n \to \infty }(a_{n})=L$ | given |
| $\varepsilon:=1$ |  |
| $\exists N:n>N\implies\vert a_{n}-L\vert<1$ |  |
| $\vert a_{n}\vert=\vert(a_{n}-L)+L\vert\leq\vert a_{n}-L \vert+\vert L\vert<1+\vert L \vert$ | triangle inequality |
| $M:=\max\{ \vert a_{1}\vert ,\vert a_{2}\vert , \dots, \vert a_{N}\vert , \vert L\vert  \}+1$ |  |
| $\vert{a_{n}}\vert<M$ |  |

## (2.22) Null * Bounded = Null 

A product of **null** and **bounded** sequences is **null** sequence

|  |  |  |
| ---- | ---- | ---- |
| 1 | $\displaystyle\lim_{ n \to \infty }a_{n}=0$ | given |
| 2 | $\vert b_{n}\vert<M$ | given |
|  | $\forall \varepsilon>0,\exists N:\forall n \in \mathbb{N},(n>N\implies \vert{a_{n}}\vert<\varepsilon)$ | by 1 |
| 3 | $\forall \varepsilon>0,\exists N:\forall n \in \mathbb{N},\left( n>N\implies \vert{a_{n}}\vert<{\color{red}\frac{\varepsilon}{M}} \right)$ | by 2.18  |
|  | $\vert a_{n}b_{n}\vert=\vert a_{n}\vert\vert b_{n}\vert<\frac{\varepsilon}{M} M=\varepsilon$ | by 2 & 3 |
|  | $\displaystyle\lim_{ n \to \infty }a_{n}b_{n}=0$ |  |

## (2.26)

Let $(a_n)$ be a convergent sequence, if $\displaystyle\lim_{ n \to \infty }{a_{n}}\neq 0$, then for almost all $n$ we have $a_{n}\neq 0$


|  |  |
| ---- | ---- |
| $\displaystyle\lim_{ n \to \infty }a_{n}=L\neq 0$ | given |
| $\varepsilon:= \vert L\vert>0$ |  |
| $\forall \varepsilon>0,\exists N:\forall n \in \mathbb{N},(n>N\implies \vert{a_{n}-L}\vert<\vert L \vert)$ | by definition |
| for almost all $n$ we have $a_{n}\neq 0$ |  |

## (2.32)

- Let $(a_n)$ and $(b_n)$ be two convergent sequences:
- Let $(x_n)$ be a sequence, where $a_{n}\leq x_{n}\leq b_{n}$ for almost all $n$, then, $\displaystyle\lim_{n \to \infty} a_n =\lim_{n \to \infty} b_n=L\implies\displaystyle\lim_{n \to \infty} x_n=L$

|  |
| ---- |
| $\displaystyle\lim_{n \to \infty} a_n =\lim_{n \to \infty} b_n=L$ |
| $\forall \varepsilon>0,\exists N_{1}:\forall n \in \mathbb{N},(n>N_{1}\implies L-\varepsilon<{a_{n}}<L+\varepsilon)$ |
| $\forall \varepsilon>0,\exists N_{2}:\forall n \in \mathbb{N},(n>N_{2}\implies L-\varepsilon<{b_{n}}<L+\varepsilon)$ |
| $N:=\max\{ N_{1},N_{2} \}$ |
| $\forall \varepsilon>0,\exists N:\forall n \in \mathbb{N},(n>N\implies L-\varepsilon<a_{n}\leq x_{n}\leq b_{n}<L+\varepsilon)$ |
| $\displaystyle\lim_{n \to \infty} x_n=L$ |

## (2.43e) 1/∞=0
 
|  |  |
| ---- | ---- |
| $\displaystyle\lim_{n \to \infty} a_n=\infty$ | given |
| $\forall K \in \mathbb{R},\exists N \in \mathbb{N}:\forall n \in \mathbb{N},(n\geq N\implies a_{n}>K)$ |  |
| $\forall K \in \mathbb{R},\exists N \in \mathbb{N}:\forall n \in \mathbb{N},\left( n\geq N\implies a_{n}<\frac{1}{K} \right)$ |  |
| $\forall K \in \mathbb{R},\exists N \in \mathbb{N}:\forall n \in \mathbb{N},\left( n\geq N\implies K<\frac{1}{a_{n}} \right)$ |  |
| #todo  |  |

## (2.47)



# Unit 3

## (3.10)

- (3.10) $\sup{(A+B)}=\sup{A}+\sup{B}$

|  |  |  |
| ---- | ---- | ---- |
|  | $\forall a \in A,a\leq \sup{A}$ |  |
|  | $\forall b \in B,b\leq \sup{B}$ |  |
|  | $a+b\leq \sup{A} +\sup{B}$ |  |
| 1 | $\sup{A} +\sup{B}$ is upper bound of $A+B$ |  |
|  | $\forall \varepsilon>0,\exists a \in A:a>\sup{A}-\frac{\varepsilon}{2}$ | by 3.9 |
|  | $\forall \varepsilon>0,\exists b \in B:b>\sup{B}-\frac{\varepsilon}{2}$ | by 3.9 |
| 2 | $\forall \varepsilon>0,\exists (a+b)\in(A+B): a+b >\sup{A}+\sup{B}-\varepsilon$ |  |
|  | $\sup{A} +\sup{B}=\sup(A+B)$ | by 3.9 using 1 & 2 |

## 3.16 & 3.17
 
 [[Monotonicity#Monotone Convergence Theorem]]

## 3.22 (Cantor's Lemma)

## 3.32 (BW)



# unit 4

## 4.30
## 4.41

## 4.42


____


# unit 5

- (5.15) **Composition Function** - if $g$ is continuous in $t_{0}$, and $f$ is continuous in $x_{0}$ where $x_{0}=g(t_{0})$, then $f(g(x))$ is continuous in $t_{0}$

## 5.29

## 5.30

## 5.35

- assuming $f$ is continuous on $I=[a,b]$
	- (5.35) Boundedness theorem (*Weierstrass 1*)
		- $f$ is **bounded** on $I=[a,b]$
		- $\exists{m,M}: \displaystyle  {\displaystyle m\leq f(x)\leq M\quad \forall x\in [a,b]}$

## 5.37

- assuming $f$ is continuous on $I=[a,b]$
	- (5.37) **Extreme value theorem** (EVT) (*Weierstrass 2*)
		- $f$ has both a maximum and a minimum on $I=[a,b]$
		- $\exists c,d\in[a,b]:\forall{x}\in[a,b],~f(c)\geq f(x) \geq{f(d)}$

# unit 6

## 6.15

# unit 7
## 7.9

# unit 8

## 8.4 (Fermat's Theorem)
## 8.5 (Rolle's Theorem)
## 8.6 (MVT-Lagrange)
## 8.9 (MVT-Cauchy - 2nd proof)
## 8.10 (Darboux's Theorem)