
# Aritmetic

$U,W\subseteq{V}$

- $U + W = \{u+w \mid u\in U , w \in W \}. \tag{4.4.1}$
- **Direct sum**:  $U\oplus{W}=V \iff U+{W}=V$ and $U \cap W=\{ 0 \}$
	- (8.3.7) if $V=U+W$, then $V=U\oplus W \iff \dim V= \dim U+\dim W$ 

# Equivalence

- Determine if two spaces are equal, $U=V$
	- Option 1: check if $U=\text{Sp}{(S)}$ is equal to $V=\text{Sp}{(T)}$
	- check if the matrix by S as rows, is ***row-equivalent*** to the matrix by T as rows (7.5.12)
	- Option 2: if $U\subseteq V$ then $U=V \iff \dim V=\dim U$. (8.3.4)


# Isomorphic Subspaces

- def
- Determine if two subspaces are isomorphic. $V\cong{W}$
	assumption: the spaces are on the same filed $F$  
	- (9.5.7, 9.5.9) $\dim{V}=\dim{W} \iff V\cong{W}$
	- (9.5.8) $\dim{V}=n\implies V\cong{F^n}$

# Dimension 

- (8.3.6) $\dim(U+W)=\dim{U}+\dim{W}-\dim(U \cap W)$
- (8.3.7) if $V=U+W$, then $V=U\oplus W \iff \dim V= \dim U+\dim W$ 
- (9.5.9) $V \cong W \iff \text{dim}{V}=\text{dim}{W}$ (on the same field, and infinite dim.)
- (9.6.1) **Rank–nullity theorem** $\text{dim}{V}=\text{dim}{(\text{Ker}{T})}+\text{dim}{(\text{Im}{T})}$. ($T:V\to W$ is lin. trans.)
- dimension of row/column space of a matrix is the rank of A
- dimension of solution sub-space of homogeneous system (nul A) (see 8.6.1)

# Linear independence

Whether $K=\set{{v}_1,\dots,{v}_k}\subseteq V$ is **linearly independent**?

- Definition: $K$ is said to be **linearly independent**, if the vector equation $\lambda_1{v}_1 + \lambda_2{v}_2 + \cdots + \lambda_k{v}_k = {0}\implies{\lambda_{1},\dots,{\lambda_{k}}}=0$. In other words, if the linear system $Ax=[v_{1},\dots, v_{k}][\lambda_{1},\dots,{\lambda_{k}}]=0$ has only the trivial solution.
- if $V$ is not the $F^n$ space, (for e.g. *matrices space* or *polynomial space*), then replace the **vecotrs** in the **coordinate vectors**. (q8.2.5, q8.4.1a, q8.4.2a)
- if $0\in{K}$, then $K$ is linearly dependent.
- $K$ is linearly independent, if and only if, there is a pivot in every column of the **REF** form of $A$. #todo 

# Span

- $\text{Sp}{(K)}=\text{Sp}{(T)}\iff{K\subseteq\text{Sp}{(T)}\land{T\subseteq\text{Sp}{(K)}}}$
- $K\subseteq{\text{Sp}{(T)}}\implies{\text{Sp}{(K)}\subseteq\text{Sp}{(T)}}$
- $K \subseteq{T}\implies{\text{Sp}{(K)}\subseteq\text{Sp}{(T)}}$

### whether a set of vectors $K$, spans the space $V$

- https://math.stackexchange.com/questions/56201/how-to-tell-if-a-set-of-vectors-spans-a-space


# Basis

## finding a basis

### basis of the **solutions sub-space of** $A\textbf{x}=\textbf{0}$ (*Homogeneous System*) 

(q8.2.4)
- Transformation $A$ to reduced row echelon form	
- find the solutions space
- find a span of the solutions space
- check if the span is linearly independent
- if so, then the span is basis of the solutions space

(q8.6.3)
- Obtain the reduced row echelon form (RREF) of $A$
- find the general solution
- extract the variables from the general solution
- the number of variables is the size of the basis
- #todo 

### basis of the row space of a matrix $B$
(q8.5.2b)

- Transformation $B$ to row echelon form $A$
- then, the **non-zero rows** of $A$ are the basis of the row space of $A$, and therefore of $B$. and their number is the rank $\rho{(B)=}\rho{(A)}$

### basis of the column space of a matrix $B$

-  the basis of **the column space** of a matrix $B$, is the basis of **the row space** of a matrix $B^t$,

### basis of the sub-space 

finding basis for $U=\text{Sp}({\set{v_{1},v_{2},\dots,v_{k}   }})\subseteq {F}^n$

reducing a span set to a basis by removing a vectors 
(q8.5.2b)

- set the ${\set{v_{1},v_{2},\dots,v_{k}   }}$ as row vector of matrix, and then follow [[#basis of the row space of a matrix $B$]] 

 **OR:**

#todo check if it's correct 
Let $(v_{1}, \dots , v_{k})$ be a list of vectors in $F^n$. To find a basis $B$ for $\text{Sp}(v_{1}, \dots , v_{k})$: 
- Put $A = [v_{1} · · · v_{k}]$ (each vector as column) in **RREF**. 
- If the $i$-th column contains a pivot, include $v_{i}$ in $B$. 


### basis of the sub-space 
basis of the sub-space $U=\text{Sp}({\set{u_{1},u_{2},\dots,u_{p}   }})$ of $V$, on field $F$ ($\dim{V}=n$)

- choose some basis $B$ of $V$. (usually the standard basis) 
- find a basis $\set{w_{1},w_{2},\dots,{w_{k}}}$ of the sub-space $W=\text{Sp}(\set{[u_{1}]_{B},[u_{2}]_{B},\dots,[u_{p}]_{B}})$ of $F^n$, 
- $w_{1},w_{2},\dots,{w_{k}}\in{F^n}$, are coordinate vectors by $B$ of $v_{1},v_{2},\dots,{v_{k}}\in{V}$. (respectively)
- $\set{v_{1},v_{2},\dots,{v_{k}}}$ are the basis of $U$

### Extending a linearly independent set to a basis by adding vectors

#todo 
- Obtain the reduced row echelon form (RREF) of the matrix as row of vectors. and then complete it to identity matrix. (the rows for the complete are the vectors for complete to basis)
- q8.3.6
- q8.6.4 

### basis for ImT

### basis for KerT

## whether a set of vectors $K$, is a basis of the space $V$

### method 1

Make sure **TWO out of three** are fulfilled (8.3.2)
1. $K$ is indep. lin. 
2. $\text{Sp}(K)=V$  (K spans V)
3. $|K|=\dim{V}$ 

### method 2

- (8.4.5) - let $B={(v_{1},v_{2},\dots,v_{n})}$ is a basis of the space $V$ ($n$-dim.), on $F$, then $B'={(u_{1},u_{2},\dots,u_{n})}$ is a basis of $V$, **iff** the transition matrix from $B$ to $B'$ is invertible.


# Coordinate vector

> q8.4.1b (matrices space), q8.4.2b (polynomial space)

- (8.4.4) Vectors are *linearly independent*, if and only if, its coordinate vectors are *linearly independent*.
- (10.2.1) coordinate vector of image - $[T(v)]_{C}=[T]^{B}_{C}[v]_{B}$

# Orthogonality 

- (d12.2.2) $\mathbf{v} \perp U$ if for all vectors $\mathbf{u} \in U$, $\mathbf{v} \cdot \mathbf{u} = 0$
- (12.2.3) let $K$ spans $U$, then $\mathbf{v} \perp U$, if and only if, $\mathbf{v} \perp K$

## Orthogonal Complement

- (d12.2.4) The **Orthogonal Complement** -  $U^{\perp}=\set{\mathbf{v}\in \mathbb{R}^n  \mid \mathbf{v} \cdot \mathbf{u} = 0, \forall{\mathbf{u} \in U }}$
	- (q12.2.7) ${U^{\perp}}\cap{U}=\{ \mathbf{0} \}$
- (12.3.1) The **row space** of $A$ and the **null space** of $A$ are orthogonal complements
- (12.3.2) The **Orthogonal Decomposition** of the Euclidean space of dimension $n$. 
	- (12.3.2a) ${U^{\perp}}\oplus{U}=\mathbb{R}^n$
	- (12.3.2a) $\dim U^{\perp}+\dim U=n$
	- (12.3.2b) $(U^\perp)^{\perp}=U$

## Orthogonal Projection

- Definition: the **orthogonal projection** of $\mathbf{a}$ onto $\mathbf{u}$ is $\frac{\mathbf{a}\cdot \mathbf{u}}{\mathbf{u}\cdot \mathbf{u}}\mathbf{u}$.
- Definition: the **orthogonal projection** of $\mathbf{a}$ onto $U\subseteq{\mathbb{R}^n}$ is the vector $$\textbf{u}=\sum^{k}_{i=1}{\frac{\mathbf{a}\cdot \mathbf{u}_{i}}{\| \textbf{u}_{i} \|^2}\textbf{u}_{i}}=\text{proj}_{U}\mathbf{a}$$
	- (where $(\mathbf{u}_{1},\dots,\mathbf{u}_{k})$ is **orthogonal** basis of $U$, and $0\neq\mathbf{a}\in{\mathbb{R}^n}$, and $\mathbf{a}=\mathbf{u}+\mathbf{v}$ where $\mathbf{u}\in{U}$ and $\mathbf{v}\in{U}^{\perp}$) (after12.3.2, 12.4.6)
	- $\mathbf{a}=\mathbf{u}+\mathbf{v}$ is the uniqe form of $\mathbf{a}$ as vector in $U$ and vector in $U^{\perp}$
	- The orthogonal projection of $\mathbf{a}$ onto $U$ is the closest vector to $\mathbf{a}$ in $U$
	- if $(\mathbf{u}_{1},\dots,\mathbf{u}_{k})$ is **orthonormal** basis of $U$, then $\textbf{u}=\sum^{k}_{i=1}{{(\mathbf{a}\cdot \mathbf{u}_{i})}\textbf{u}_{i}}=\text{proj}_{U}\mathbf{a}$
- Projection Theorem - if $\mathbf{v}$ and $\mathbf{u}$ are vectors in $\mathbb{R}^n$, and $\mathbf{u}\neq \mathbf{0}$, then $\mathbf{v}$ can be expressed in excatly one way in the form $\mathbf{v}=t\mathbf{u}+\mathbf{w}$, where $t$ is a scalar, and $\mathbf{w}\perp\mathbf{u}$.

- (12.5.1) $\{ \mathbf{u}_{1},\dots,\mathbf{u}_{k} \}$ is orthogonal set in $\mathbb{R}^n$. and $P(\mathbf{a})$ is the orthogonal projaction of some vector $\mathbf{a}\in \mathbb{R}^n$ onto $\text{Sp}(\{ \mathbf{u}_{1},\dots,\mathbf{u}_{k} \})$, and $\mathbf{v}=\mathbf{a}-P(\mathbf{a})$, then:
	1.  $\mathbf{v}\perp{\{ \mathbf{u}_{1},\dots,\mathbf{u}_{k} \}}$, and $\mathbf{v}\perp{\text{Sp}(\{ \mathbf{u}_{1},\dots,\mathbf{u}_{k} \})}$
	2. $\mathbf{v}=\mathbf{0}\iff \mathbf{a}\in{\text{Sp}(\{ \mathbf{u}_{1},\dots,\mathbf{u}_{k} \})}$


> [!example] Methods
> - given subspace $U$, find the orthogonal projection of $\mathbf{a}$ on $U^{\perp}$. (e2023a.85.q1b)
> 	- find basis for $U$
> 	- find basis for $U^{\perp}$
> 	- normalize this $U^{\perp}$ basis into $(\mathbf{u}_{1},\dots,\mathbf{u}_{k})$
> 	- then $\textbf{u}=\sum^{k}_{i=1}{{(\mathbf{a}\cdot \mathbf{u}_{i})}\textbf{u}_{i}}=\text{proj}_{U^{\perp}}\mathbf{a}$


## orthogonal set

- (d12.4.1a) let $K=\{ \textbf{u}_{1}, \dots,\textbf{u}_{k} \} \subseteq\mathbb{R}^n$. we say that $K$ is a **orthogonal set**, if $\textbf{0}\notin{K}$, and $\forall{j\neq i}:\textbf{u}_{i}\cdot\textbf{u}_{j}=0$
- (12.4.2) Every orthogonal set in $\mathbb{R}^n$ is independent set
- (q12.4.3a) Every orthogonal set in $\mathbb{R}^n$ has at most $n$ vectors

## orthonormal set

- (d12.4.1b) $K=\{ \textbf{u}_{1}, \dots,\textbf{u}_{k} \}$ is **orthonormal set** if, $\| \textbf{u}_{i} \|=1$ for each $i$, ($1\leq i\leq k$)
- (q12.4.2) **Normalizing** - if $K=\{ \mathbf{u}_{1}, \dots,\textbf{u}_{k} \}$ is orthogonal set, then $L=\{ \frac{\textbf{u}_{1}}{\|\textbf{u}_{1} \|},\dots,\frac{\textbf{u}_{k}}{\|\textbf{u}_{k} \|} \}$ is orthonormal set, and $\text{Sp}(K)=\text{Sp}(L)$
- **The normalized vector** $\mathbf{\hat{u}}$ of a non-zero vector $\mathbf{{u}}$ is the unit vector in the direction of $\mathbf{{u}}$. i.e. $\mathbf{\hat{u}} = \frac{\mathbf{u}}{\|\mathbf{u}\|}$
- A **Unit vector** is a vector $\textbf{v}$ such that $\| \textbf{v} \|=1$

- (12.4.5) let $B=(u_{1}, \dots ,u_{n})$ ordered basis of $\mathbb{R}^n$, then the following properties are equivalence:
	- $B$ is orthonormal basis
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



___
