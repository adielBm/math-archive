
$$\large A\subseteq\mathbb{R}$$
# Greatest element & least element

- max(A), min(A)

# Upper & lower bounds


### Upper bound

- (d3.1) real number $c$ is called **upper bound** of $A$, if $\forall a\in{A}: c\geq a$ 

### Lower bound 

- (d3.1) real number $c$ is called **lowe bound** of $A$, if $\forall a\in{A}: c\leq a$
### Supremum (Least-upper-bound)

- definitions
	- $c=\sup{A}$. ($c$ is the **supremum** of $A$)
	- (d3.7) $c$ is minimal upper bound of $A$
	- (3.9) (1.) $c$ is an upper bound of $A$ (2.) $\forall\varepsilon>0 \;\exists{x\in{A}}:x>c-\varepsilon$
	- (3.9) (1.) $c$ is an upper bound of $A$ (2.) $c\leq d$ for all upper bounds $d$ of $A$
- Theorems
	- (3.6 **Least-upper-bound property**, see note below) 
		- If $A$ is **non-empty** and **bounded above**, then $A$ has **supremum**
	- (3.8) if $A$ has maximum, then $\sup{A}=\max{A}$
	- (3.10) $\sup{(A+B)}=\sup{A}+\sup{B}$
	- $a<b\implies \sup(a,b)=b$


> *Least-upper-bound property* (3.6) is follow from the completeness axiom. but the opposite is also true. 
> Also **many books** called to Least-upper-bound property as (a1.52) **completeness axiom**. (see q3.14).
> The rationals $\mathbb{Q}$ **does not have** the least upper bound property.

### Infimum (Greatest-lower-bound)

- definitions
	- $y=\inf{A}$
	- (d3.12) $y$ is maximal lower bound of $A$
	- (q3.11a) $y$ is lower bound of $A$, and for every $\varepsilon>0$ there exists $x\in{A}$ such that $x<y+c$
- theorems 
	- (3.11) if $A$ is **non-empty** and **bounded below**, then $A$ has **infimum**
	- $a<b\implies \inf(a,b)=a$
	- (3.13b) if $A$ has minimum, then $\inf{A}=\min{A}$
	- (3.10) $\sup{(A+B)}=\sup{A}+\sup{B}$

### theorems

- (q3.13) if $A$ is **non-empty** and **bounded**, then $\inf{A}\leq\sup{A}$

# Closed & Open Sets

- open set
	- equivalent **definitions** 
		- $\forall{a\in{A}},{\exists{\varepsilon>0}}:(a-\varepsilon,a+\varepsilon)\subseteq{A}$
		- $A\subseteq\mathbb{R}$ is **open set** 
	- theorems 
		- d

- closed set
	- equivalent definitions
		- $A\subseteq\mathbb{R}$ is **closed set** 
		- if given convergent sequence $(x_{n})$ of $A$ elements, we have also $\lim_{ n \to \infty }x_{n}\in{A}$
		- $A^{\complement}=\mathbb{R}\setminus{A}$ is *open set*
	- theorems 
		- The set of subsequential limits is closed
		- $[a,b]$ is closed