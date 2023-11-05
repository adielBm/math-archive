# Axioms

## Field Axioms
  
- Addition
	- Associative $(a+b)+c = a+(b+c)$
	- Commutative $a+b=b+a$
	- Identity $\exists{0}:a + 0 = 0 + a = a$
	- Inverse $\forall a \in \mathbb{F}, \exists b \in \mathbb{F} : a + b = 0$
- Multiplication
	- Associative $a · (b · c) = (a · b) · c$
	- Commutative $a · b = b · a$
	- Identity $∃ 1 \neq 0 : a · 1 = 1 · a = a$
	- Inverse $\forall a \in \mathbb{F} \setminus \{0\}, \exists b \in \mathbb{F} : a \cdot b = 1$
- Distributive $a · (b + c) = a · b + a · c$

## Order Axioms

1. (Trichotomy Law, (asymmetric+connected)) **one and only one** of the following three statements is true: $a\neq{b},\quad{a<b},\quad{b<a}$ 
2. (Transitivity) $a<b\land b<c\implies a<c$
3. $a<b\implies a+c<b+c$
4. $a<b \land c>0\implies ac<bc$



## Completeness Axiom

- (a1.52) if $\emptyset\neq A,B\subseteq\mathbb{R}$ such that $\forall{a}\in{A}$ and $\forall{b}\in{B}$ we have $a\leq b$. then there exists $x\in\mathbb{R}$ such that:
	- $\forall{a}\in{A}$, $a\leq{x}$
	- $\forall{b}\in{B}$, $x\leq{b}$

>See 3.16

# Theorems & Properties

- Theorems follow from the *field axioms*
	- (1.25) Cancellation law (addition) $a+c=b+c\implies a+b$
	- (1.26) Cancellation law (multiplication) $c\neq 0$ and $ac=bc\implies ab$
	- (1.27) additive inverse uniqueness 
	- (1.28) Multiplicative inverse uniqueness 


- Theorems
	- #todo 1.36 etc...


- (q1.61a) sum of rational & irrational is irrational
	- $x\in\mathbb{R\setminus{Q}}\land q\in\mathbb{Q}\implies{x+q\in{\mathbb{R\setminus{Q}}}}$
- (q1.61c) product of nonzero rational & irrational is irrational
	- $x\in\mathbb{R\setminus{Q}}\land 0\neq{q}\in\mathbb{Q}\implies{xq\in{\mathbb{R\setminus{Q}}}}$
## Roots

- (1.55) For every real $c>0$ and every natural $n$ there is **one and only one** real positive $x\geq 0$ such that $x^n=c$. 
	- (d1.56) $x$ is called the $n$th root of $c$. and noted $x=\sqrt[n]{c}$


## Archimedean property

- (1.61) for each $0<a,b\in\mathbb{R}$ there exists $n\in\mathbb{N}$ such that $na>b$

## Absolut Value 


## Density

- (d1.65) $A\subseteq\mathbb{R}$ is dense in $\mathbb{R}$ if for every reals $x<y$ there exists $a\in{A}$ such that $a\in(x,y)$
	- (1.66) $\mathbb{Q}$ is dense in $\mathbb{R}$ (between any two distinct real numbers there is a rational number. )
	- (q1.62) $\mathbb{R\setminus{Q}}$ is dense in $\mathbb{R}$. (between any two distinct real numbers there is an irrational number. )

- (q1.57) there exist infinite rationals between any two reals

## Inequalities

- (1.43) **Bernoulli's Inequality** If $x>-1$ then $({1 + x})^n \ge 1 + n x$ for all $n \in \mathbb{N}$
- (1.49) **Triangle inequality** - $|{a+b}|\leq{|{a}|+|b|}$
- (1.59) **Mean Inequalities** $HM\leq GM\leq AM$. $x_{1},\dots ,x_{n}$ are positive reals
  $$\frac{n}{\sum^{n}_{i=1}{\frac{1}{x_{i}}}}\quad\leq\quad{\sqrt[n]{ \prod^{n}_{i=1}x_{i}}}\quad\leq\quad \frac{1}{n}\sum^{n}_{i=1}x_{i}$$

