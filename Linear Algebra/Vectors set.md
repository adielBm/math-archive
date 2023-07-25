$$\large{K=\set{{v}_1,\dots,{v}_m}\subseteq V}, \quad \dim{V}=n$$
- $A_{R}$ is $K$'s vectors as **rows** 
- $A_{C}$ is $K$'s vectors as **comluns** 
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

Whether $K$ is a basis of $V$ ?

Make sure **TWO out of three** are fulfilled (8.3.2)
1. $K\text{ is linearly {\bf independent}}$
2. $\text{Sp}(K)=V$  (K spans V)
3. $m=n$ 

### method 2

- (8.4.5) - let $B={(v_{1},v_{2},\dots,v_{n})}$ is a basis of the space $V$ ($n$-dim.), on $F$, then $B'={(u_{1},u_{2},\dots,u_{n})}$ is a basis of $V$, **iff** the transition matrix from $B$ to $B'$ is invertible.


### finding a basis

basis of the $\text{null}{(A_{C})}$ 

(q8.2.4)
- find span to $\text{null}({\text{RREF}(A)})$
- reduce the span until it will be also linearly independent

(q8.6.3)
- find the general solution of ${\text{RREF}(A)}$
- extract the variables from the general solution
- the number of variables is the size of the basis
- #todo 


- (q8.5.2b) A basis of $\text{row-space}({A})$. 
	- The **non-zero** rows of $\text{REF}(A)$ are a basis of $\text{row-space}({A})$.
-  A basis of $\text{column-space}({A})$.
	- The **non-zero** rows of $\text{REF}(A^t)$ are a basis of $\text{column-space}({A})$.

### basis of the sub-space 

finding basis for $U=\text{Sp}({\set{v_{1},v_{2},\dots,v_{k}   }})\subseteq {F}^n$

reducing a span set to a basis by removing a vectors 
(q8.5.2b)

- set the ${\set{v_{1},v_{2},\dots,v_{k}   }}$ as row vector of matrix, and then follow basis of the row space of a matrix $B$ 

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


