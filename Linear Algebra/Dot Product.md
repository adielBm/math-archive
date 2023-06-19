
>$\textbf{a},\textbf{b}, \textbf{c}, \textbf{v}\in \mathbb{R}^n$
>$U$ is subspace of $\mathbb{R}^n$
>$t\in \mathbb{R}$

- $\textbf{0}\cdot\textbf{a}=\textbf{a}\cdot\textbf{0}=0$
- $\textbf{a}\cdot\textbf{b}=\textbf{b}\cdot\textbf{a}$
- $(\textbf{a}+\textbf{b})\cdot{\textbf{c}}=\textbf{a}\cdot\textbf{c}+\textbf{b}\cdot\textbf{c}$
- $(t\textbf{a})\cdot\textbf{b}=t(\textbf{a}\cdot\textbf{b})$
- $\textbf{a}\cdot\textbf{a}\geq 0$
- $\textbf{a}\cdot\textbf{a}= 0 \iff \textbf{a}=\textbf{0}$

# Norm of a Vector

- (d12.1.3) - $\| \textbf{a} \|=\sqrt{\textbf{a} \cdot \textbf{a}}=\sqrt{ \sum_{i=1}^{n}a_{i}^2 }$
- (q12.1.4) $\|\textbf{a} \|=0 \iff \textbf{a}=\textbf{0}$
- (q12.1.5) $\|t \textbf{a} \|=|t|\cdot\| \textbf{a} \|$
- Cauchy–Schwarz inequality (12.1.4) $|\textbf{a}\cdot\textbf{b}| \leq  \| \textbf{a} \| \cdot{\| \textbf{b} \|}$
- (q12.1.7) $|\textbf{a}\cdot\textbf{b}| =  \| \textbf{a} \| \cdot{\| \textbf{b} \|} \iff \textbf{a},\textbf{b}$ are linearly inpendent 
- (q12.1.8) Triangle inequality for vectors $\| \textbf{a} + \textbf{b} \| \leq \| \textbf{a} \| +{\| \textbf{b} \|}$

# Orthogonality 

- (d12.2.1) Two vectors $\textbf{a}$ and $\textbf{b}$ are called orthogonal if $\textbf{a}\cdot\textbf{b}=0$ (This relationship is denoted $\textbf{a}\perp\textbf{b}$)
- (q12.2.3) Generalized Theorem of Pythagoras - if $\textbf{a}\perp\textbf{b}$, then  $\| \textbf{a} + \textbf{b} \|^2 = \| \textbf{a} \|^2 +{\| \textbf{b} \|}^2$
- (d12.2.2) $\mathbf{v} \perp U$ if for all vectors $\mathbf{u} \in U$, $\mathbf{v} \cdot \mathbf{u} = 0$
- (12.2.3) let $K$ spans $U$, then $\mathbf{v} \perp U$, if and only if, $\mathbf{v} \perp K$
- (d12.2.4) **Orthogonal Complement** -  $U^{\perp}=\set{\mathbf{v}\in \mathbb{R}^n  \mid \mathbf{v} \cdot \mathbf{u} = 0, \forall{\mathbf{u} \in U }}$
	- (q12.2.7) ${U^{\perp}}\cap{U}=\{ \mathbf{0} \}$
	- (12.3.2b) $(U^\perp)^{\perp}=U$
	- (13.3.2a) ${U^{\perp}}\oplus{U}=\mathbb{R}^n$
	- (13.3.2a) $\dim U^{\perp}=n-\dim U$
- (12.3.1) the solution space of $Ax=0$ is the orthogonal complement of the row space of $A$.
- (d12.4.1a) let $K=\{ \textbf{u}_{1}, \dots,\textbf{u}_{k} \} \subseteq\mathbb{R}^n$. we say that $K$ is a **orthogonal set**, if $\textbf{0}\notin{K}$, and $\forall{j\neq i}:\textbf{u}_{i}\cdot\textbf{u}_{j}=0$
- (d12.4.1b) $K=\{ \textbf{u}_{1}, \dots,\textbf{u}_{k} \}$ is **orthonormal set** if, $\| \textbf{u}_{i} \|=1$ for each $i$, ($1\leq i\leq k$).
- (q12.4.2) Normalizing if $K=\{ \mathbf{u}_{1}, \dots,\textbf{u}_{k} \}$ is orthogonal set, then $L=\{ \frac{\textbf{u}_{1}}{\|\textbf{u}_{1} \|},\dots,\frac{\textbf{u}_{k}}{\|\textbf{u}_{k} \|} \}$ is orthonormal set, and $\text{Sp}(K)=\text{Sp}(L)$
- **The normalized vector** $\mathbf{\hat{u}}$ of a non-zero vector $\mathbf{{u}}$ is the unit vector in the direction of $\mathbf{{u}}$. i.e. $\mathbf{\hat{u}} = \frac{\mathbf{u}}{\|\mathbf{u}\|}$
- A **Unit vector** is a vector $\textbf{v}$ such that $\| \textbf{v} \|=1$
- (12.4.2) Every orthogonal set in $\mathbb{R}^n$ is independent set
- (q12.4.3a) Every orthogonal set in $\mathbb{R}^n$ has at most $n$ vectors
- (12.4.5) let $B=(u_{1}, \dots ,u_{n})$ orderd basis of $\mathbb{R}^n$, then the following properties are equivalence:
	- $B$ is orthonormal basis
	- $\textbf{a}=\sum^{n}_{i=1}{(\mathbf{a\cdot u}_{i})\cdot{\mathbf{u}_{i}}}$
	- $\mathbf{a\cdot b}=\sum^{n}_{i=1}{(\mathbf{a\cdot u}_{i})\cdot(\mathbf{b\cdot u}_{i})}$
	- $\| \textbf{a} \|^2=\sum^n_{i=1}(\mathbf{a\cdot u}_{i})^2$
- (q12.4.10) #todo generalition of 12.4.5 for orthogonal bases
- (12.4.6) #todo 






