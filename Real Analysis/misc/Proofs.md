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

| Proof by Contradiction | implied by |
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

|  |  | implied by |
| ---- | ---- | ---- |
| 1 | $\displaystyle\lim_{ n \to \infty }a_{n}=0$ | given |
| 2 | $\vert b_{n}\vert<M$ | given |
|  | $\forall \varepsilon>0,\exists N:\forall n \in \mathbb{N},(n>N\implies \vert{a_{n}}\vert<\varepsilon)$ | by 1 |
| 3 | $\forall \varepsilon>0,\exists N:\forall n \in \mathbb{N},\left( n>N\implies \vert{a_{n}}\vert<{\color{red}\frac{\varepsilon}{M}} \right)$ | by 2.18  |
|  | $\vert a_{n}b_{n}\vert=\vert a_{n}\vert\vert b_{n}\vert<\frac{\varepsilon}{M} M=\varepsilon$ | by 2 & 3 |
|  | $\displaystyle\lim_{ n \to \infty }a_{n}b_{n}=0$ |  |

## (2.26)

Let $(a_n)$ be a convergent sequence, if $\displaystyle\lim_{ n \to \infty }{a_{n}}\neq 0$, then for almost all $n$ we have $a_{n}\neq 0$


|  | implied by |
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

|  |  | implied by |
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

## (4.30) (ε, δ)-definition ≡ Heine's definition

|  | 1st Direction: (ε, δ)-definition => Heine's definition | implied by |
| ---- | ---- | ---- |
|  | $\displaystyle\lim_{ x \to x_{0} }f(x)=L$ | given |
| 1 | ${\forall \varepsilon >0,\,\exists \delta >0,\,\forall x\in \mathbb {R} ,(\,0<\vert x-x_{0}\vert<\delta \implies \vert f(x)-L\vert<\varepsilon )}$ | by (ε, δ)-definition |
|  | Let $(x_{n})$ a sequence such that $x_{n}\neq x_{0}$ for all $n$ and $\displaystyle\lim_{ n \to \infty }x_{n}=x_{0}$ |  |
| 2 | $\forall\varepsilon>0,\exists N \in \mathbb{N}: \forall n \in\mathbb{N}\left(n \geq N \implies 0 <\vert x_n - x_{0}\vert < \varepsilon \right)$ | by def & $x_{n}\neq x_{0}$ |
|  | $\forall n>N, \vert f(x_n) - L\vert < \varepsilon$ | by 1 & 2  |
|  | $\displaystyle\lim_{ n \to \infty } f(x_{n})=L$ |  |



|  | 2nd Direction: Heine's => (ε, δ); (Proof by Contradiction) |  |
| ---- | ---- | ---- |
|  |  | given |



## 4.41

- $\displaystyle \lim_{ x \to x_{0} }f(x), \lim_{ x \to x_{0} }g(x)$ are defined
	- $\displaystyle{\color{gray}\exists{\varepsilon>0}:\forall x \in N^{*}_{\varepsilon}(x_{0}),\,}f(x)\leq g(x)\implies \lim_{ x \to x_{0} }f(x)\leq \lim_{ x \to x_{0} }g(x)$

|  |  |  |
| ---- | ---- | ---- |
|  | $\displaystyle \lim_{ x \to x_{0} }f(x), \lim_{ x \to x_{0} }g(x)$ are defined | given-1 |
|  | $\displaystyle{\color{gray}\exists{\varepsilon>0}:\forall x \in N^{*}_{\varepsilon}(x_{0}),\,}f(x)\leq g(x)$ | given-2 |
| 1 | let's define $x_{n}=x_{0}+1/n$ |  |
|  | $\displaystyle\lim_{ x \to x_{0} }f(x)=\lim_{ n \to \infty }f(x_{n}),\,\lim_{ x \to x_{0} }g(x)=\lim_{ n \to \infty }g(x_{n})$ | by 1 & Heine & given-1 |
|  | $\displaystyle\lim_{ n \to \infty }x_{n}=x_{0}$ | by 1 |
|  | for almost all $n$: $x_{n}\in N_{\varepsilon}(x_{0})$ |  |
|  | for almost all $n$: $x_{n}\in N^{*}_{\varepsilon}(x_{0})$ |  |
|  | for almost all $n$: $f(x_{n})\leq g(x_{n})$ | by given-2 |
|  | $\displaystyle\lim_{ n \to \infty }f(x_{n})\leq \lim_{ n \to \infty }g(x_{n})$ | by 2.31 |
|  | $\displaystyle\lim_{ x \to x_{0} }f(x)\leq \lim_{ x \to x_{0} }g(x)$ |  |

## 4.42

- (4.42) $\displaystyle{\color{gray}\exists{\varepsilon>0}:\forall x \in N^{*}_{\varepsilon}(x_{0}),\,}f(x)< g(x)\impliedby\lim_{ x \to x_{0} }f(x)< \lim_{ x \to x_{0} }g(x)$

|  |  |  |
| ---- | ---- | ---- |
|  | $\displaystyle \lim_{ x \to x_{0} }f(x), \lim_{ x \to x_{0} }g(x)$ are defined | given-1 |
|  | $\displaystyle \lim_{ x \to x_{0} }f(x)< \lim_{ x \to x_{0} }g(x)$ | given-2 |
|  | let's defind $h(x)=g(x)-f(x)$ |  |
|  | $L=\displaystyle\lim_{ x \to x_{0} }h(x)=\lim_{ x \to x_{0} }g(x)-\lim_{ x \to x_{0} }f(x)>0$ |  |
|  | #todo  |  |

#todo 

____


# unit 5

- (5.15) **Composition Function** - if $g$ is continuous in $t_{0}$, and $f$ is continuous in $x_{0}$ where $x_{0}=g(t_{0})$, then $f(g(x))$ is continuous in $t_{0}$

## 5.29

- assuming $f$ is continuous on $I=[a,b]$
	- (5.29) **Bolzano's Theorem**
		- $f(a)\cdot f(b)<0\implies \exists c\in(a,b):f(c)=0$

|  | Statement | Implied By |
| ---- | ---- | ---- |
|  | $f$ is continuous on $I=[a,b]$ | Given-1 |
|  | $f(a)\cdot f(b)<0$ | Given-2 |


## (5.30) Existence of root for odd polynomial

> it's sufficient that we'll proof for a odd polynomial that its leading coefficient is $a_{n}=1$, because if $a_{n}\neq 1$ then $P(x)/a_{n}$ is odd polynomial that its leading coefficient is $1$ and its roots are equal to $P$'s roots

|  | implied by |
| ---- | ---- |
| $P=x^n+b_{n-1}x^{n-1}+\dots+b_{1}x^1+b_{0}$ | given-1 |
| $\deg{P}=n$ is odd | given-2 |
| $P=x^n\left( 1+\frac{b_{n-1}}{1}+\dots+\frac{b_{1}}{x^{n-1}}+\frac{b_{0}}{x^{n}} \right)$ | by given-1 |
| $g(x):=\left( 1+\frac{b_{n-1}}{1}+\dots+\frac{b_{1}}{x^{n-1}}+\frac{b_{0}}{x^{n}} \right)$ | notation |
| $P(x)=x^n{g(x)}$ |  |
| $\displaystyle\lim_{ x \to \infty }g(x)=\displaystyle\lim_{ x \to -\infty }g(x)=1$ |  |
| $\exists M \in \mathbb{R}^+ : \forall x, \, \vert{x}\vert > M \implies g(x) > 0$ |  |
| $\exists a<0:P(a)=a^n\cdot{g(a)}<0$ | $g$ is positive; $n$ is odd  |
| $\exists b>0:P(b)=b^n\cdot{g(b)}>0$ | $g$ is positive |
| $P(a)\cdot P(b)<0$ |  |
| $\exists c\in(a,b):P(c)=0$ | by 5.29 |


## (5.35) W1

- assuming $f$ is continuous on $I=[a,b]$
	- (5.35) Boundedness theorem (*Weierstrass 1*)
		- $f$ is **bounded** on $I=[a,b]$
		- $\exists{m,M}: \displaystyle  {\displaystyle m\leq f(x)\leq M\quad \forall x\in [a,b]}$



|  | Proof by Contradiction | Implied By |
| ---- | ---- | ---- |
| Given-1 | $f$ is continuous on $I=[a,b]$ |  |
|  | $f$ is **not bounded** above on $I=[a,b]$ | Assume by contradiction |
|  | $\forall n \in \mathbb{N}, \exists x_{n} \in(a,b):f(x_{n})>n$ |  |
|  | let's de |  |
|  |  |  |
|  |  |  |
|  |  |  |
|  |  |  |
|  |  |  |
|  |  |  |

#todo 

## (5.37) W2 (EVT)

- assuming $f$ is continuous on $I=[a,b]$
	- (5.37) **Extreme value theorem** (EVT) (*Weierstrass 2*)
		- $f$ has both a maximum and a minimum on $I=[a,b]$
		- $\exists c,d\in[a,b]:\forall{x}\in[a,b],~f(c)\geq f(x) \geq{f(d)}$

>this's a proof for maximum (for minimum is analogous)

| Step | Statement | Implied By |
| ---- | ---- | ---- |
|  | $f$ is continuous on $I=[a,b]$ | Given |
|  | $f$ is bounded on $I=[a,b]$ | (5.35) W1 |
|  | $M:=\sup f([a,b])$ |  |
|  | $\forall\varepsilon>0,\exists{y\in{f([a,b])}}:y>M-\varepsilon$ | by 3.9 |
|  | $\forall\varepsilon>0,\exists{x_{0}\in{[a,b]}}:f(x_{0})>M-\varepsilon$ |  |
|  | $\forall n \in\mathbb{N},\exists{x_{n}\in[a,b]}:f(x_{n})>M-\frac{1}{n}$ |  |
|  | $\forall n \in\mathbb{N},\exists{x_{n}\in[a,b]}:f(x_{n})\leq M$ |  |
| 1 | $\displaystyle\lim_{ n \to \infty }f(x_{n})=M$ | by squeeze |
|  | $(x_{n})$ is bounded |  |
|  | $(x_{n})$ has a convergent subsequence $(x_{n_{k}})$ | by BW (3.32) |
|  | $x_{0}:=\displaystyle\lim_{ k \to \infty }x_{n_{k}}$ |  |
|  | $a\leq x_{0} \leq b$ |  |
|  | $\displaystyle\lim_{ k \to \infty }f(x_{n_{{k}}})=M$ | by 1 and 3.25 |
|  | $f(x_{0})=\displaystyle\lim_{ k \to \infty }f(x_{n_{k}})=M$ | by 5.27 |
|  | $x_{0}$ is maximum point of $f$ on $[a,b]$ |  |

# Unit 6

## 6.15
- (6.15) $\displaystyle\lim_{ n \to \infty }\left(a_{n}^{b_{n}}\right)=\left(\lim_{ n \to \infty }a_{n}\right)^{\left(\displaystyle\lim_{ n \to \infty }b_{n}\right)}$ (assuming $\lim a_{n}>0$, and $\lim b_{n}\in\mathbb{R}$)


|  | Statement | Implied By |
| ---- | ---- | ---- |
| Given-1 | $\displaystyle\lim_{ n \to \infty }a_{n}=a>0$ |  |
| Given-2 | $\displaystyle\lim_{ n \to \infty }r_{n}=r\in \mathbb{R}$ |  |
|  | for almost all $n$ we have $a_{n}>0$ | by Given-1 |
|  | $a_{n}^{r_{n}}$ is defined |  |
| 1 | $a_{n}^{r_{n}}=e^{r_{n}\ln a_{n}}$ |  |
|  | $\displaystyle\ln{a}=\ln{(\lim_{ n \to \infty }a_{n})}=\lim_{ n \to \infty }\ln a_{n}$ | $\ln$ is continuous at $\displaystyle\lim_{ n \to \infty }a_{n}=a$ |
|  | $\displaystyle\lim_{ n \to \infty }r_{n}\ln{a}=\lim_{ n \to \infty }r_{n}\lim_{ n \to \infty }\ln a_{n}$ | multiply by $\displaystyle\lim_{ n \to \infty }r_{n}=r$ |
| 2 | $\displaystyle{r}\ln{a}=\lim_{ n \to \infty }r_{n}\ln a_{n}$ |  |
|  | $\displaystyle\lim_{ n \to \infty }a_{n}^{r_{n}}\stackrel{\small(1)}{=}\lim_{ n \to \infty }e^{r_{n}\ln a_{n}}=e^{r\ln{a}}=a^r$ |  by 1; by 2; $e^x$ is continuous at $r \ln a$;   |

#todo 

# Unit 7
## (7.9) Differentiability Implies Continuity

(7.9) if $f$ is differentiable at $x_{0}$, then it is continuous at $x_{0}$

|  | Statement | Implied By |
| ---- | ---- | ---- |
| Given-1 | $f$ is differentiable at $x_{0}$ |  |
| 1 | $\displaystyle  f'(x_{0})=\lim_{x\to{x_{0}}}{\frac{f(x)-f(x_{0})}{x-x_{0}}}$ |  |
|  | $f(x)-f(x_{0})=\frac{f(x)-f(x_{0})}{x-x_{0}}(x-x_{0})$ |  |
|  | $\displaystyle\lim_{ x \to x_{0} }(f(x)-f(x_{0}))=\lim_{ x \to x_{0} }\left( \frac{f(x)-f(x_{0})}{x-x_{0}}(x-x_{0}) \right)$ |  |
|  | $\displaystyle\lim_{ x \to x_{0} }(f(x)-f(x_{0}))=\lim_{ x \to x_{0} }\frac{f(x)-f(x_{0})}{x-x_{0}}\lim_{ x \to x_{0} }(x-x_{0})$ |  |
|  | $\displaystyle\lim_{ x \to x_{0} }(f(x)-f(x_{0}))=f'(x_{0})\cdot0=0$ | by 1 |
|  | $\displaystyle\lim_{ x \to x_{0} }f(x)=f(x_{0})$ |  |
|  | $f$ is continuous at $x_{0}$ |  |
# Unit 8

## 8.4 (Fermat's Theorem)

- $f$ is defined on an interval $I$ and $x_{0}\in I$
	- **Fermat's theorem** (8.4) - Let $x_{0}$ a local extremum point of $f$. if $f$ is differentiable at $x_{0}$, then $f'(x_{0})=0$

>This a proof for local **maximum** point, a proof for local **minimum** point is similar.

|  | Statement | Implied By |
| ---- | ---- | ---- |
| Given-1 | $f$ is defined on an interval $I$ and $x_{0}\in I$ |  |
| Given-2 | $x_{0}$ a local **maximum** point of $f$ |  |
| Given-3 | $f$ is differentiable at $x_{0}$ |  |
| 1 | $\exists N_{\delta}(x_{0}):\forall{x},f(x)\leq f(x_{0})$ | Given-2 |
| $\forall h:\vert{h}\vert<\delta$ | $x_{0}+h\in N_{\delta}(x_{0})$ | by 1; |
|  | $f(x_{0}+h)\leq f(x_{0})$ |  |
|  | $f(x_{0}+h)-f(x_{0})\leq 0$ |  |
| if $h>0$ | $\frac{f(x_{0}+h)-f(x_{0})}{h}\leq 0$ |  |
| if $h<0$ | $\frac{f(x_{0}+h)-f(x_{0})}{h}\geq 0$ |  |
|  | $f'(x_{0})=f_{-}'(x_{0})=f_{+}'(x_{0})$ is defined | Given-3; 7.12 |
|  | $f'(x_{0})=f'_{+}(x_{0})=\displaystyle\lim_{ h \to 0^+ }\frac{f(x_{0}+h)-f(x_{0})}{h}\leq 0$ |  |
|  | $f'(x_{0})=f'_{-}(x_{0})=\displaystyle\lim_{ h \to 0^- }\frac{f(x_{0}+h)-f(x_{0})}{h}\geq 0$ |  |
| **Conclusion** | $f'(x_{0})=0$ |  |


## 8.5 (Rolle's Theorem)

|  | Statement | Implied By |
| ---- | ---- | ---- |
| Given-1 | $f$ is continuous on $[a,b]$ |  |
| Given-2 | $f$ is differentiable on the $(a,b)$ |  |
| Given-3 | $f(a)=f(b)$ |  |
|  | $m=\min f([a,b])$, $M=\max f([a,b])$ | by W2 (5.37) |
| if $m=M$ | $\forall x \in[a,b],f(x)=M$ |  |
|  | $\forall c \in(a,b),f'(c)=0$ | derivative of constant function |
| if $m\neq M$ | $\exists x_{1},x_{2}:f(x_{1})=m,f(x_{2})=M$ |  |
|  | $f(x_{1})\neq f(x_{2})$ |  |
|  | at least one of $x_{1},x_{2}$ is an inferior point | because Given-2: $f(a)=f(b)$ |
|  | $\exists c\in(a,b):f'(c )=0$ | by Fermat (8.4); Given-2;  |


## (8.6) Lagrange's MVT


|  | Statement | Implied By |
| ---- | ---- | ---- |
| Given-1 | $f$ is continuous on $[a,b]$ |  |
| Given-2 | $f$ is differentiable on the $(a,b)$ |  |
|  | $\ell(x):=\left( \frac{f(b)-f(a)}{b-a} (x-a)+f(a)\right)$ |  |
|  | $g(x):=f(x)-\ell(x)$ |  |
|  | $g$ is continuous on $[a,b]$ | Given 1; difference of contentious functions; |
|  | $g$ is differentiable on the $(a,b)$ | Given 2; difference of differentiable functions; |
|  | $g(a)=f(a)-\ell(a)=0$ |  |
|  | $g(b)=f(b)-\ell(b)=0$ |  |
| $\exists c \in(a,b):$ | $g'(c)=0$ | by Rolle's Theorem; |
|  | $f'(c)-\frac{f(b)-f(a)}{b-a} =0$ |  |
|  | $f'(c)=\frac{f(b)-f(a)}{b-a}$ |  |


## (8.9) Cauchy's MVT (2nd proof)




## (8.10) Darboux's Theorem


|  | Statement | Implied By |
| ---- | ---- | ---- |
| Given-1 | $f$ is differentiable on $[a,b]$ |  |
| Given-2 | $f'(a)<t<f'(b)$ |  |
|  | $H(x):=f(x)-tx$ |  |
|  | $H$ is differentiable and continuous on $[a,b]$  |  |
|  | $\exists c\in[a,b]:\forall{x}\in[a,b],~H(c)\leq H(x)$ | by EVT-W2 |
|  | #todo show $c$ IS NOT ENDPOINT!!! |  |
|  |  |  |
|  | $c\in(a,b)$  |  |
|  | $H'(c)=0$ | by Fermat; |
|  | $H'(x)=f'(x)-t$ |  |
|  | $H'(c)=f'(c)-t=0$ |  |
|  | $f'(c)=t$ |  |


____


# Limits

## $\lim_{n\to\infty}(1+\frac{1}{n^2})^n = 1$

| Step |  | Implied By |
| ---- | ---- | ---- |
| 1. | $\lim_{n\to\infty}(1+\frac{1}{n})^n = e$ |  |
| 2. | $\exists K > 1: \forall n>0,1 < \left(1+\frac{1}{n}\right)^n < K$ |  |
| 3. | $1 < \left(1+\frac{1}{n^2}\right)^n = \left(\left(1+\frac{1}{n^2}\right)^{n^2}\right)^{1/n} < K^{1/n}$ |  |
| 4. | $\lim_{n\to\infty}\left(1+\frac{1}{n^2}\right)^n=\lim_{n\to\infty}\left(\left(1+\frac{1}{n^2}\right)^{n^2}\right)^{1/n}$ |  |
| 5. | $\lim_{n\to\infty}\left(1+\frac{1}{n^2}\right)^{n^2} = 1$ | Consequence of given limit |
| 6. | $\lim_{n\to\infty}\left(1+\frac{1}{n^2}\right)^n=\lim_{n\to\infty}1^{1/n}$ | Substituting the result from step 5 |
| 7. | $\lim_{n\to\infty}1^{1/n} = 1$ | Limit of a constant raised to the power of $1/n$ is 1 |
| 8. | $\lim_{n\to\infty}\left(1+\frac{1}{n^2}\right)^n = 1$ | Final result |

The inequality $1 < \left(1+\frac{1}{n}\right)^n < K$ is a consequence of the fact that the limit $\lim_{n\to\infty}\left(1+\frac{1}{n}\right)^n$ exists and is equal to the mathematical constant $e$.

Here's a more detailed explanation:

1. **Given**: $\lim_{n\to\infty}\left(1+\frac{1}{n}\right)^n = e$

2. **Consequence**: Since the limit is equal to $e$, there exists some positive constant $K > 1$ such that for every positive integer $n$, the expression $\left(1+\frac{1}{n}\right)^n$ is always between $1$ and $K$. In other words, $1 < \left(1+\frac{1}{n}\right)^n < K$ for all positive integers $n$.

This is a general property of the limit $e$. It implies that the sequence $\left(1+\frac{1}{n}\right)^n$ is bounded between $1$ and some constant $K$ for sufficiently large $n$.

Now, when proving $\lim_{n\to\infty}\left(1+\frac{1}{n^2}\right)^n = 1$, you can use this property to establish that $\left(1+\frac{1}{n^2}\right)^n$ is also bounded and, therefore, converges to $1$ as $n$ approaches infinity.