## Row equivalence

- row equivalence is equivalence relation

whether two matrices are row equivalent #todo 

## Rank of Matrix $\rho{(A_{{m \times n}})}$

- other notation: $\text{rank}{(A)}$
- (d8.5.4) the rank $\rho{(A)}$ is the dim. of the row/column space of $A$
- $\rho(A)$ is the number of the non-zero rows of REF of $A$
- $\rho(A)$ is the number of pivots in the RREF of $A$. 
- (q8.5.4) $\rho{(A)}=\rho{(A^t)}$
- (q8.5.5) $\rho{(A_{m \times n})}\leq\min{\{ m,n \}}$
- (q8.5.6) $\rho{(AB)}\leq\min{\{ \rho{(A)}, \rho{(B)} \}}$
- (q8.5.7a) let $A_{m \times n}$, and $B_{n}$ invertible matrix, then $\rho(AB)=\rho(A)$ 
- (q8.5.7b) let $A_{m \times n}$, and $B_{m}$ invertible matrix, then $\rho(BA)=\rho(A)$ 
- (8.6.1) **Rank–nullity** theorem  $n=\dim(\text{nul}{(A)})+\rho(A)$
- Only a zero matrix has rank zero. #todo 
- row equivalent matrices must have the same rank #todo 
- rank of **square matrix**
	- (q8.5.8a) let $A$ square matrix of order $n$, then $\rho(A)=n \iff |A|\neq 0$  
	- (q10.5.3) $A,B$ are square matrices of order $n$, then $\rho{(AB)}\geq \rho(A)+\rho(B)-n$


## Transformation matrix

Matrix Representations of Linear Transformation

- (d10.1.1) $T:V\to W$, and $B=(v_{1},\dots,v_{n})$ and $C=(w_{1},\dots,w_{n})$ are bases of $V$ and $W$. (respectively) 
$$[T]_{C}^{B}=\left[\begin{array}{ccc} | & & | \\ [T({v_{1}})]_{C} & \cdots & [T( {v_{n}})]_{C} \\ | & & | \end{array} \right]_{m\times n}$$

# Square Matrices

Let $A$ be an $n \times n$ square matrix.

## Invertibility 

- **Procedure:** determine whether a square matrix $A$ is invertible and, if so, find $A^{−1}$: 
	- Form the augmented matrix $[A | I_{n}]$ and put it into RREF. 
	- If the RREF has the form $[I_{n} | B]$, then $A$ is invertible and $B=A^{−1}$. 
	- else, if the matrix in the left half of the RREF is not $I_{n}$, then $A$ is singular. 
- **Theorem 3.10.6**: Let $A$ be a $n$-ordered square matrix over a field $F$. The following statements are **equivalent**:
	- $A$ is row-equivalent to the identity matrix $I$
	- The RREF of $A$ is $I$
	- The columns of A are linearly independent.
	- The rows of A are linearly independent.
	- The columns of A span $F^n$
	- The rows of A span $F^n$
	- The columns of A is a basis $F^n$
	- The rows of A a basis $F^n$
	- #todo 
	- (4.4.1) The determinant of A is nonzero: $\det{A}\neq0$
	- (4.4.1, and q11.3.1) The number $0$ **is not an eigenvalue** of $A$. 
	- (q8.5.8b) $A$ has a full rank: $\rho(A)=n$
	- (10.5.1, and 9.6.2) $A$ has trivial kernel: $\ker(A)=\{ 0 \}$

### Inversion matrix $A^{-1}$

let A square matrix, find $A^{-1}$, see [[Decision problems#Invertibility]]

> **WolframAlpha** `inverse [matrix]`

## Determinant $|A|$

- **Procedure:** 
	1. convert $A$ into an upper triangular matrix $B$ via row operations of **switching rows**, and **adding multiplication of another row**. (but **NOT** scaling of row by scalar)
		- Note: if during the row operations we find zero-row, then $\det A=0$
	2. let $k$ be the number of times two rows are switched
	3. $\det{A}=(−1)^kb_{11} · · · b_{nn}$
- **Theorems:**
	- (10.7.3) **similar matrices** have the same determinant
	- (q11.3.1) $\det{A}=0$, if and only if, $\lambda=0$ is eigenvalue of $A$
	- Row Operations
		- If a multiple of one row of $A$ is **added** to another row to produce a matrix $B$, then $\det B=\det A$
		- If two rows of $A$ are **interchanged** to produce $B$, then $\det B=-\det A$
		- if one row of $A$ is **multiplied** by $k$ to produce $B$, then $\det B=k \cdot \det A$ 
	- $\det A$ is equal to the product of its eigenvalues (see q11.4.7)

## Characteristic polynomial 
$$\det \left( \lambda I -A \right)$$
- (q11.4.6-7) finding coefficients of **the characteristic polynomial** of a matrix
	- The **free coefficient** of the characteristic polynomial of $A$ is $\det-A =(-1)^n\det{A}$
	- 

## Eigenvalues and Eigenvectors

### Finding Eigenvalues and Eigenvectors

**Procedure**: Finding Eigenvalues and Eigenvectors

1. First, find the eigenvalues $\lambda$ of $A$ by solving the **characteristic equation** $\det \left( \lambda I -A \right) = 0$.
2. For each $\lambda$, find the basic eigenvectors $X \neq 0$ by finding the basic solutions to $\left( \lambda I - A \right) X = 0$.
To verify your work, make sure that $AX=\lambda X$ for each $\lambda$ and associated eigenvector $X$.

**Theorems**:
- if $\lambda$ is an eigenvalue of A, then the union of the zero vector $\mathbf{0}$ and the set of all eigenvectors corresponding to eigenvalues $\lambda$ is known as the **eigenspace** of $A$ associated with eigenvalue $\lambda$.
- (11.4.1) $\lambda$ is an eigenvalue of $A$, if and only if, $\lambda$ is a solution of the **characteristic equation** $\det(\lambda I-A)=0$
- similar matrices have the same eigenvalues (11.3.3), and the same algebraic multiplicities of eigenvalues ( #todo  )
- the sum of eigenvalues of $A$ equals to $\text{tr}A$ #todo 
- the multiplication of eigenvalues of $A$ equals to $\text{det}A$ #todo  
- the eigenvalues of diagonal matrix $\text{diag}{(\lambda_{1},\dots,\lambda_{{n}})}$, are $\lambda_{1},\dots,\lambda_{{n}}$   #todo 

### whether a scalar is an eigenvalue of $A$

- (d11.3.1) the scalar $\lambda$ is called an **eigenvalue** of $A$, if there is a non-zero **column** vector $v$, such that: $Av=\lambda{v}$. (in such case, $v$ is called an **eigenvector** of $A$ that related to the eigenvalue $\lambda$.) 
- (q11.3.2a) if $\lambda$ is an eigenvalue of $A$, then for each $\mu$, $\mu\lambda$ is an eigenvalue of $\mu A$
- (q11.3.2b) if $\lambda$ is an eigenvalue of $A$, then , $\lambda^k$ is a eigenvalue of $A^k$. (for each natural $k$ )
- (11.4.1) $\lambda$ is an eigenvalue of $A$, if and only if, $\lambda$ is a solution of the **characteristic equation** $\det(\lambda I-A)$ is $0$
-  #todo - $\lambda$ is an eigenvalue of $A$, if and only if, the system of equations $(\lambda I-A)v=0$ has nontrivial solutions.

### Algebraic & geometric multiplicity

- (d11.5.2) The multiplicity of an eigenvalue $\lambda$ as a root of the characteristic equation is **the algebraic multiplicity** of $\lambda$ 
-  The dimension of the eigenspace corresponding to $\lambda$ is called **the geometric multiplicity** of $\lambda$
- (q11.5.2) the **geometric multiplicity** of $\lambda$ equals to $n-\rho(\lambda I-A)$
- (11.5.3, q11.5.3)  $1\leq$ the **geometric multiplicity** $\leq$ the **algebraic multiplicity**
- finding the algebraic multiplicity of eigenvalue #todo 
- finding the geometric multiplicity of eigenvalue #todo 

## Trace 

- $\text{tr} A$ is the sum of its eigenvalues #todo 
- (10.7.6) $\text{tr}(AB)=\text{tr}(BA)$
- (10.7.5) similar matrices have the same trace
- $\text{tr}(A+B)=\text{tr}(A)+\text{tr}(B)$ 
- $\text{tr}(cA)=c\text{tr}(A)$ #todo 
- $\text{tr}(A)=\text{tr}(A^t)$ #todo 

## Similarity

- Similarity is an equivalence relation on the space of square matrices. (wikipedia)
- matrices are similar, if and only if, they represent the same linear operator with respect to (possibly) different bases. (wikipedia)
- (d10.7.1) If $A$ and $B$ are square matrices, then we say that $A$ **is similar to** $B$ if there is an invertible matrix $M$ such that $A=M^{-1}BM$ 
- (10.7.2) $A$ and $B$ square matrices of order $n$ on filed F, represent the same linear transformation (n-dim. and on F), if and only if, they $A$ and $B$ are similar.
- #todo to show that two matrices are similar, show that are similar to the same diagonal matrix
- #todo let $A$ and $B$ are diagonalizable, and they both have the same eigenvalues, then they're similar (because similarity is transitive) 
- #todo let $A$ and $B$ are diagonalizable, and they both have the same characteristic polynomial, then they're similar (because similarity is transitive) 


shared properties: determinant (10.7.3), trace (10.7.5), eigenvalues (11.3.3), algebraic multiplicities of eigenvalues ( #todo  ),  characteristic polynomial (11.4.3)
	
## Diagonalizable

- (d11.3.4) if there exists an $n \times n$ invertible matrix $M$, such that $M^{-1}AM$ is a diagonal matrix, then $A$ is a **diagonalizable matrix**
- (d11.3.4) $A$ is diagonalizable, if and only if, $A$ is similar to a diagonal matrix
- (11.3.5) $T:V\to V$ is diagonalizable, if and only if, $A$ is diagonalizable
- (11.3.6) if $A$ has $n$ **distinct** eigenvalues, then $A$ is **diagonalizable matrix**
- (11.3.7) $M$ is an $n \times n$ invertible matrix.  $M^{-1}AM$ is a diagonal matrix, (i.e. $A$ is diagonalizable), if and only if, the columns of $M$ are $n$ independent linearly eigenvectors of $A$. ^[in such case,  if the columns of $M$ are $v_{1},\dots,v_{n}$, and for each $i$ ($1\leq i\leq n$), $v_i$ is a eigenvector of $A$ that's related to the eigenvalue $\lambda_{i}$ , then $M^{-1}AM=\text{diag}{(\lambda_{1},\dots,\lambda_{{n}})}$]
- (q11.3.7) $A$ on filed $F$ is diagonalizable, if and only if, $F^n$ has a basis that consists of eigenvectors of $A$ 
- (q11.4.10) $A$ is diagonalizable, if and only if, $A^t$ is diagonalizable
- (11.5.4') The matrix $A$ is diagonalizable, if and only if, (i) the characteristic polynomial factors completely into linear factors and (ii) the algebraic multiplicity of each eigenvalue of $A$ is equal to its geometric multiplicity.
- #todo The matrix $A$ is diagonalizable, if and only if, the sum of the dimensions of the eigenspaces equals to $n$
- #todo $A^k=M{D}^{k}M^{-1}$, ($D$ is a diagonal matrix)

## Symmetric matrix

- (d3.2.6) ${A}\text{ is symmetric} \iff A=A^t$

>**WolframAlpha** is `[matrix]` a symmetric matrix?

## Change of Basis matrix (Transition matrix) 
also *change-of-coordinates matrix*

**Definition:**
- (d8.4.6) Let $B=(v_{1},\dots ,v_{n})$ and $B'=(u_{1},\dots ,u_{n})$ bases of $V$. if $$\begin{align}
u_{1} &= a_{11}v_{1}+\dots+a_{n1}v_{n} \\ \vdots \notag \\ u_{n} &= a_{1n}v_{1}+\dots+a_{nn}v_{n}  \\ \end{align}$$then $$M=\begin{bmatrix} a_{11}  & \dots & a_{1n} \\    \vdots &  \ddots & \vdots \\ a_{n1}  & \dots & a_{nn} \end{bmatrix}$$ is the **transition matrix** from basis $B$ to basis $B'$. 
- the **transition matrix** from basis $B$ to basis $B'$ is the matrix that its columns are the coordinate vectors of the $B'$ vectors by $B$.

**Properties:**
- transition matrix is square matrix of $n$-order, which $n=\dim V$
- transition matrix is invertible matrix (by 8.4.5)
- #todoooo   The transition matrix is actually the representative matrix of the identity map with respect to the two bases.

**Theorems:**
- (8.4.8) if $A$ is square matrix, and $[v]_{B}=A[v]_{B'}$ then $A$ is the transition matrix from $B$ to $B'$.  
- (8.4.8) if $M$ is the transition matrix from $B$ to $B'$, then $M^{-1}$ is the transition matrix from $B'$ to $B$


>[!example] Finding the transition matrix from an old basis to a new basis 
>1. Form the partitioned matrix $[\text{new basis} | \text {old basis}]$ in which the basis vectors (or coordinate vectors) are in column form. 
>2. Use elementary row operations to reduce the matrix in Step 1 to **RREF**.
>3. The resulting matrix will be $[{I} | \text{transition matrix from old to new}]$ where $I$ is an identity matrix.
>4. Extract the matrix on the right side of the matrix obtained in Step 3. 

### Transition matrix from a basis B to the standard basis

- if $B=(v_{1}, v_{2},\dots,v_{n})$, then $[v_{1}|v_{2}|\dots|v_{n}]$ is the transition matrix from B to the standard basis
