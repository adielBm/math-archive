$$\large{K=\set{{v}_1,\dots,{v}_m}\subseteq V}, \quad \dim{V}=n$$
- $A$ is $K$'s vectors as **rows** 
- $A^t$ is $K$'s vectors as **comluns** 
- $r=\text{rank}(A)$
- $B$ is some basis of $V$ 

# Linear independence

Whether $K$ is **linearly independent**?

- **Definition**: $K$ is said to be **linearly independent**, if: $$\lambda_1{v}_1 + \lambda_2{v}_2 + \cdots + \lambda_m{v}_m = {0}\implies{\lambda_{1},\dots,{\lambda_{m}}}=0$$ 
- In other words, if the linear system $Ax=[v_{1},\dots, v_{m}][\lambda_{1},\dots,{\lambda_{m}}]=0$ has only the trivial solution. ($A$ is vectors as comluns)


- ($A$ is $K$'s vectors as **rows**) $\text{rank}({A})=m\leq n\iff K\text{ is linearly {\bf independent}}$.
- if $m=n$, then, $K\text{ is linearly {\bf independent}}\iff A \text{ is {\bf invertible} matrix}$. ($A$ is vectors as comluns/rows)
- $0\in{K}\implies K\text{ is linearly {\bf dependent}}$
- $m>n\implies K\text{ is linearly {\bf dependent}}$

- (8.4.4) $K\text{ is linearly {\bf independent}}\iff \{ [v_{1}]_{B},\dots,[v_{m}]_{B} \}\text{ is linearly {\bf independent}}$
- $K$ is linearly independent, if and only if, there is a pivot in every column of the **REF** form of $A$. #todo 

# Span

Whether $K$, spans $V$ ?

- $K\text{ spans }V \iff \text{rank}(\text{REF}(A))=\dim{V}$.   ($A$ is $K$'s vectors as rows)
- $K\text{ spans }V \iff A\mathbf{x}=\mathbf{b}\text{ is consistent}$.   ($A$ is $K$'s vectors as columns)
- $B\subseteq{\text{Sp}{(K)}}\implies{K\text{ spans }V}$. (where $\text{Sp}({B})=V$)
- $m<n\implies K\text{ is {\bf not} span }V$

**Theorems:**
- $\text{Sp}{(K)}=\text{Sp}{(T)}\iff{K\subseteq\text{Sp}{(T)}\land{T\subseteq\text{Sp}{(K)}}}$
- $K\subseteq{\text{Sp}{(T)}}\implies{\text{Sp}{(K)}\subseteq\text{Sp}{(T)}}$
- $K \subseteq{T}\implies{\text{Sp}{(K)}\subseteq\text{Sp}{(T)}}$

# Basis

Definitions of **basis**. The following statements are **equivalent**:
- $K$ is a basis of $V$
- every element of $V$ may be written in a unique way as a finite linear combination of elements of $K$.
- **two** out of three are fulfilled (8.3.2)
	1. $K\text{ is linearly {\bf independent}}$
	2. $\text{Sp}(K)=V$  (K spans V)
	3. $m=\dim V$ 
- (8.4.5) $m=\dim V$, and the transition matrix from some basis $B$ to $K$ is invertible

### Bases for the Fundamental Spaces

- A basis of $\text{row-space}({A})=\text{Sp}(K)$
	- The **non-zero** rows of $\text{REF}(A)$ (q8.5.2b)
	- The $r$ columns in $A^t$, such that in $\text{RREF}(A^t)$ are contain a pivot.
-  A basis of $\text{column-space}({A})$.
	- The **non-zero** rows of $\text{REF}(A^t)$
	- The $r$ columns in $A$, such that in $\text{RREF}(A)$ are contain a pivot.
- A basis of the $\text{null}{(A)}$ 
	- The $n-r$ vectors that span the solution space of $(\text{RREF}(A))\mathbf{x}=\mathbf{0}$. 
- A basis of the $\text{null}{(A^t)}=\text{left-null}{(A^t)}$ 
	- The $m-r$ vectors that span the solution space of $(\text{RREF}(A^t))\mathbf{x}=\mathbf{0}$. 


### Extending a linearly independent set to a basis by adding vectors

#todo 
- Obtain the reduced row echelon form (RREF) of the matrix as row of vectors. and then complete it to identity matrix. (the rows for the complete are the vectors for complete to basis)
- q8.3.6
- q8.6.4 

- #todo  basis for ImT
- #todo  basis for KerT



# Orthogonality  

## Orthogonal set

- (d12.4.1a) let $K=\{ \textbf{u}_{1}, \dots,\textbf{u}_{k} \} \subseteq\mathbb{R}^n$. we say that $K$ is a **orthogonal set**, if $\textbf{0}\notin{K}$, and $\forall{j\neq i}:\textbf{u}_{i}\cdot\textbf{u}_{j}=0$
- (12.4.2) Every orthogonal set in $\mathbb{R}^n$ is independent set
- (q12.4.3a) Every orthogonal set in $\mathbb{R}^n$ has at most $n$ vectors

### Orthogonal basis



## Orthonormal set

- (d12.4.1b) $K=\{ \textbf{u}_{1}, \dots,\textbf{u}_{k} \}$ is **orthonormal set** if, $\| \textbf{u}_{i} \|=1$ for each $i$, ($1\leq i\leq k$)
- (q12.4.2) **Normalizing** - if $K=\{ \mathbf{u}_{1}, \dots,\textbf{u}_{k} \}$ is orthogonal set, then $L=\{ \frac{\textbf{u}_{1}}{\|\textbf{u}_{1} \|},\dots,\frac{\textbf{u}_{k}}{\|\textbf{u}_{k} \|} \}$ is orthonormal set, and $\text{Sp}(K)=\text{Sp}(L)$
- **The normalized vector** $\mathbf{\hat{u}}$ of a non-zero vector $\mathbf{{u}}$ is the unit vector in the direction of $\mathbf{{u}}$. i.e. $\mathbf{\hat{u}} = \frac{\mathbf{u}}{\|\mathbf{u}\|}$
- A **Unit vector** is a vector $\textbf{v}$ such that $\| \textbf{v} \|=1$

### Orthonormal basis

- (12.4.5) let $B=(u_{1}, \dots ,u_{n})$ ordered basis of $\mathbb{R}^n$, then the following properties are equivalence:
	- $B$ is **orthonormal basis**
	- $\textbf{a}=\sum^{n}_{i=1}{(\mathbf{a\cdot u}_{i})\cdot{\mathbf{u}_{i}}}$
	- $\mathbf{a\cdot b}=\sum^{n}_{i=1}{(\mathbf{a\cdot u}_{i})\cdot(\mathbf{b\cdot u}_{i})}$
	- $\| \textbf{a} \|^2=\sum^n_{i=1}(\mathbf{a\cdot u}_{i})^2$
- (q12.4.10) #todo generalition of 12.4.5 for orthogonal bases

## **Gram–Schmidt process** (12.5.2) 

Convert a basis $\{ \mathbf{u}_{1},\dots,\mathbf{u}_{k} \}$ into an orthogonal basis $\{ \mathbf{v}_{1},\dots,\mathbf{v}_{k} \}$:

$$\mathbf{v}_{1}=\mathbf{u}_{1}$$
$$\mathbf{v}_{i}=\mathbf{u}_{i}-\frac{\mathbf{u}_{i}\cdot\mathbf{v}_{1}}{{\| \mathbf{v}_{1} \|^2}}\mathbf{v}_{1}-\frac{\mathbf{u}_{i}\cdot\mathbf{v}_{2}}{{\| \mathbf{v}_{2} \|^2}}\mathbf{v}_{2}-\dots-\frac{\mathbf{u}_{i}\cdot\mathbf{v}_{i-1}}{{\| \mathbf{v}_{i-1} \|^2}}\mathbf{v}_{i-1}$$

- during the computation you can multiple $\mathbf{v}_{i}$ by a scalar (note before q12.5.4)
- To convert the orthogonal basis into an orthonormal basis see (q12.4.2)
- for dependent set see q12.5.3
- expanding orthogonal set of $k<n$ vectors into orthogonal basis see q12.5.4


