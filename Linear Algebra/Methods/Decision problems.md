# Matrices 

### two matrices are row equivalent

#todo 

## Invertibility 

- **Procedure:** determine whether a square matrix $A$ is invertible and, if so, find $A^{−1}$: 
	- Form the augmented matrix $[A | I_{n}]$ and put it into RREF. 
	- If the RREF has the form $[I_{n} | B]$, then $A$ is invertible and $B=A^{−1}$. 
	- else, if the matrix in the left half of the RREF is not $I_{n}$, then $A$ is singular. 
- **Theorem 3.10.6**: Let $A$ be a $n$-ordered square matrix over a field $F$. The following statements are equivalent:
	- $A$ is row-equivalent to the identity matrix $I$
	- The RREF of $A$ is $I$
	- The columns of A are linearly independent.
	- The rows of A are linearly independent.
	- The columns of A span $F^n$
	- The rows of A span $F^n$
	- #todo 
	- (4.4.1) The determinant of A is nonzero: $|A|\neq0$
	- (q8.5.8b) $A$ has a full rank: $\rho(A)=n$
	- (10.5.1, and 9.6.2) $A$ has trivial kernel: $\ker(A)=\{ 0 \}$


## Matrix similarity

- (d10.7.1) If $A$ and $B$ are square matrices, then we say that $A$ **is similar to** $B$ if there is an invertible matrix $M$ such that $A=M^{-1}BM$ 
- (10.7.2) $A$ and $B$ square matrices of order $n$ on filed F, represent the same linear transformation (n-dim. and on F), if and only if, they $A$ and $B$ are similar.

shared properties: determinant (10.7.3), trace (10.7.5), eigenvalues (11.3.3), characteristic polynomial (11.4.3)

## diagonalizable
- $A$ is a $n \times n$ squere matrix. 
	- (d11.3.4) if there exists an $n \times n$ invertible matrix $M$, such that $M^{-1}AM$ is a diagonal matrix, then $A$ is **diagonalizable matrix**
	- (d11.3.4) $A$ is diagonalizable, if and only if, $A$ is similar to a diagonal matrix
	- (11.3.5) $T:V\to V$ is diagonalizable, if and only if, $A$ is diagonalizable
	- (11.3.6) if $A$ has $n$ **distinct** eigenvalues, then $A$ is **diagonalizable matrix**
	- (11.3.7) $M$ is an $n \times n$ invertible matrix.  $M^{-1}AM$ is a diagonal matrix, (i.e. $A$ is diagonalizable), if and only if, the columns of $M$ are $n$ indpendent linearly eigenvectors of $A$. ^[in such case,  if the columns of $M$ are $v_{1},\dots,v_{n}$, and for each $i$ ($1\leq i\leq n$), $v_i$ is a eigenvector of $A$ that's related to the eigenvalue $\lambda_{i}$ , then $M^{-1}AM=\text{diag}{(\lambda_{1},\dots,\lambda_{{n}})}$]
	- (q11.3.7)

### eigenvalues ans eigenvectors 
- $A$ is a $n \times n$ squere matrix. 
	- (d11.3.1) the scaler $\lambda$ is called **eigenvalue** of $A$, if there is a non-zero **column** vector $v$, such that: $Av=\lambda{v}$. And $v$ is called **eigenvector** of $A$ that related to the eigenvalue $\lambda$. 

# Linear Systems

## consistent linear system

- Rouché–Capelli theorem (8.6.2) - A system of linear equations with $n$ variables has a solution if and only if the rank of its coefficient matrix $A$ is equal to the rank of its augmented matrix $[A|b]$. That is $\rho([A|B])=\rho(A)$

# Linear independence

### Set of vectors $K=\set{{v}_1,\dots,{v}_k}$, is a linearly independent
- by the defintion, $K$ is linearly independent, if  $\lambda_1{v}_1 + \lambda_2{v}_2 + \cdots + \lambda_k{v}_k = {0}\implies{\lambda_{1},\dots,{\lambda_{k}}}=0$.
- in other words, check if the linear sys. has the only the trivial solution.

> q8.4.1a (matrices space), q8.4.2a (polynomial space)

####  Set of matrices, is linearly in/dependent
- q8.2.5 (is dependent)
- q8.4.1a (is independent)

## in the $F^n$ space

To check whether a list $(v_{1}, \dots , v_{k})$ in $F^n$ is linearly independent: 
- Put the matrix $A=[v_{1} \cdots v_{k}]$ (each vector as column) in **REF**. 
- $(v_{1}, \dots , v_{k})$ in $F^n$ is linearly independent **if and only if** there is a pivot in every column of the **REF**. 

# Spaces 

### Two spaces are equal, $U=V$

- Option 1: check if $U=\text{Sp}{(S)}$ is equel to $V=\text{Sp}{(T)}$
	- check if the matrix by S as rows, is ***row-equivalent*** to the matrix by T as rows (7.5.12)
- Option 2: if $U\subseteq V$ then $U=V \iff \dim V=\dim U$. (8.3.4)

### Two vector spaces are isomorphic, $V\cong{W}$

assumption: the spaces are on the same filed $F$  

- (9.5.7, 9.5.9) $\dim{V}=\dim{W} \iff V\cong{W}$
- (9.5.8) $\dim{V}=n\implies V\cong{F^n}$

# Basis

## Set of vectors $K$, is a basis of the space $V$

### method 1

Make sure **TWO out of three** are fulfilled (8.3.2)
1. $K$ is indep. lin. 
2. $\text{Sp}(K)=V$  (K spans V)
3. $|K|=\dim{V}$ 

### method 2

- (8.4.5) - let $B={(v_{1},v_{2},\dots,v_{n})}$ is a basis of the space $V$ ($n$-dim.), on $F$, then $B'={(u_{1},u_{2},\dots,u_{n})}$ is a basis of $V$, **iff** the transition matrix from $B$ to $B'$ is invertible.

# Span

#### Set of vectors $K$, spans the space $V$

https://math.stackexchange.com/questions/56201/how-to-tell-if-a-set-of-vectors-spans-a-space

# Linear Transformation

### transformation is a linear transformation

given $T:V\to W$
- firstly, check if $T(0_{V})=0_{W}$. 
	- if not, then it's not linearly (9.1.2a). 
	- else, check by d9.1.1, or equivalently by 9.1.3
		- (9.1.3)  $T(\lambda_{1}v_{1}+\lambda_{2}v_{2})=\lambda_{1}T(v_{1})+\lambda_{2}T(v_{2})$

>q9.4.1

### two linear transformations are equel 

> 9.4.1

### isomorphism
showing whether $T:V\to W$ is isomorphism from $V$ to $W$
- (9.6.2) injective $\iff$ surjective $\iff$ isomorphism. (for $V,W$ with the same dim)
- (10.5.2) if $[T]^B_{C}$ is invertible, then $T$ is isomorphism

### Diagonalizability

- (d11.1.1) $T:V\to V$ is **diagonalizable**, if there is a basis for $V$, such that the matrix of of $T$ (by this basis), is dianogal.
- (11.2.5) let $T$ is lin. trans. of dim $n$. if $T$ has $n$ **distinct** eigenvalues, then $T$ is diagonalizable
#todo  https://textbooks.math.gatech.edu/ila/diagonalization.html


### eigenvalues ans eigenvectors 

- (d11.2.1) the scaler $\lambda$ is called **eigenvalue** of $T$, if there is a non-zero vector $v \in V$, such that: $T(v)=\lambda{v}$. And $v$ is called **eigenvector** of $T$ that related to the eigenvalue $\lambda$. 

