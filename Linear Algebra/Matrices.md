
## Row Echelon form (REF)

- (1.11.1) every REF matrix is row row equivalence to the RREF matrix
- (8.5.1) The nonzero rows of REF matrix are a basis for its row space.

### Reduced Row Echelon form (RREF)



## Row equivalence

- row equivalence is equivalence relation

whether two matrices are row equivalent #todo 

## Rank

- **Notation**: $\text{rank}{(A)}=\rho{(A)}$
- (d8.5.4) $\rho{(A)}=\dim(\text{row-space(A)})=\dim(\text{column-space(A)})$
- The rank is the maximal number of linearly independent row vectors
- $\rho(A)$ is the number of the non-zero rows of REF of $A$
- $\rho(A)$ is the number of pivots in the RREF of $A$.
- (q8.5.4) $\rho{(A)}=\rho{(A^t)}$
- (q8.5.5) $\rho{(A_{m \times n})}\leq\min{\{ m,n \}}$
- (q8.5.6) $\rho{(AB)}\leq\min{\{ \rho{(A)}, \rho{(B)} \}}$
- (q8.5.7a) let $A_{m \times n}$, and $B_{n}$ invertible matrix, then $\rho(AB)=\rho(A)$ 
- (q8.5.7b) let $A_{m \times n}$, and $B_{m}$ invertible matrix, then $\rho(BA)=\rho(A)$ 
- (8.6.1) **Rank–nullity** theorem  $\rho(A)+\dim(\text{nul}{(A)})=n$
- Only a zero matrix has rank zero. #todo 
- row equivalent matrices must have the same rank #todo 
	- rank of **square matrix**
	- (q8.5.8a) let $A$ square matrix of order $n$, then $\rho(A)=n \iff |A|\neq 0$  
	- (q10.5.3) $A,B$ are square matrices of order $n$, then $\rho{(AB)}\geq \rho(A)+\rho(B)-n$

## Nulity 

- (8.6.1) $\mathrm{nullity}(A)=\dim{\mathrm{(null(A))}}=n-\rho({A})$

## Transformation matrix

Matrix Representations of Linear Transformation

- (d10.1.1) $T:V\to W$, and $B=(v_{1},\dots,v_{n})$ and $C=(w_{1},\dots,w_{n})$ are bases of $V$ and $W$. (respectively) 
$$[T]_{C}^{B}=\left[\begin{array}{ccc} | & & | \\ [T({v_{1}})]_{C} & \cdots & [T( {v_{n}})]_{C} \\ | & & | \end{array} \right]_{m\times n}$$



## Transpose

- (3.2.4)  $(A^t)^t=A$
- $(A+B)^t=A^t+B^t$
- $(AB)^t=B^tA^t$
- $(cA)^{t}=cA^{t}$
- 

# Square Matrices

Let $A$ be an $n \times n$ square matrix.

## Invertibility 

- **Theorem 3.10.6**: Let $A$ be a $n$-ordered square matrix over a field $F$. The following statements are **equivalent**:
	- $A$ is an **invertible matrix**
	- $A$ can be expressed as a finite product of elementary matrices.
	- $A$ is row-equivalent to the identity matrix $I$
	- There exists a $B$ such that $BA=I$
	- There exists a $B$ such that $AB=I$
	- There exists a $B$ such that $AB=BA=I$, (in such case $A^{-1}=B$, and $B^{-1}=A$) ()
	- $A$ is row-equivalent to $I$.
	- $A$ is column-equivalent to $I$.
	- The RREF of $A$ is $I$
	- The columns of A are linearly independent.
	- The rows of A are linearly independent.
	- The columns of A span $F^n$
	- The rows of A span $F^n$
	- The columns of A is a basis $F^n$
	- The rows of A a basis $F^n$
	- $A^t$ is an **invertible matrix** (in such case $(A^t)^{-1}=(A^{-1})^{t}$) (3.8.4b)
	- (4.4.1) The determinant of A is nonzero: $\det{A}\neq0$
	- (4.4.1, and q11.3.1) The number $0$ **is not an eigenvalue** of $A$. 
	- (q8.5.8b) $A$ has a full rank: $\rho(A)=n$
	- (10.5.1, and 9.6.2) $A$ has trivial kernel: $\ker(A)=\{ 0 \}$
	- The linear transformation mapping $\mathbf{x}$ to $A\mathbf{x}$ is **surjective**; that is, the equation $A\mathbf{x}=\mathbf{b}$ has at least one solution for each $\mathbf{b}$ in $F^n$.
	- The linear transformation mapping $\mathbf{x}$ to $A\mathbf{x}$ is **injective**; that is, the equation $A\mathbf{x}=\mathbf{b}$ has at most one solution for each $\mathbf{b}$ in $F^n$.
	- The linear transformation mapping $\mathbf{x}$ to $A\mathbf{x}$ is **bijective**; that is, the equation $A\mathbf{x}=\mathbf{b}$ has exactly one solution for each $\mathbf{b}$ in $F^n$. ($A\mathbf{x}=\mathbf{b}\implies \mathbf{x}=A^{-1}\mathbf{b}$)

- (4.5.2) $A,B$ are square matries, and $AB=I$, then $A$ and $B$ are both invetible, and $A^{-1}=B$, and $B^{-1}=A$, and $AB=BA=I$
- (3.8.3) if $A$ is invertible, then $AB=AC\implies B=C$, and $BA=CA\implies B=C$
- (3.8.4c) if $A,B$ are invertible (the same order), then $AB$ is also invertible. (in such case $(AB)^{-1}=B^{-1}A^{-1}$) 
- (3.8.4d) if $A$ is invertible, and $s\neq 0$, then $sA$ is also invertible. (in such case $(sA)^{-1}=\frac{1}{s}A^{-1}$)


> [!example] **Procedure:** determine whether a square matrix $A$ is invertible and, if so, find $A^{−1}$: 
>	- Form the augmented matrix $[A | I_{n}]$ and put it into RREF. 
>	- If the RREF has the form $[I_{n} | B]$, then $A$ is invertible and $B=A^{−1}$. 
>	- else, if the matrix in the left half of the RREF is not $I_{n}$, then $A$ is singular. 

> **WolframAlpha** `inverse [matrix]`

## Elementary matrix

- $A$ is called an **elementary matrix** if it can be obtained from an identity matrix by performing a single elementary row operation. 
- Every elementary matrix is invertible, and the inverse is also an elementary matrix. 

## Determinant 

- $\det A=|A|$ 
- **Theorems:**
	- (4.5.1) $\det (AB)=\det (A) \det (B)$
	- (4.3.1) $\det (A)=\det(A^t)$
	- (4.3.5) if $A$ has two equal rows (or colmuns), then $\det A=0$
	- (4.3.8) if $A_{n}=[a_{ij}]$ is a triangular matrix, then $\det A=a_{11}a_{22} \cdots a_{nn}$
	- (10.7.3) **similar matrices** have the same determinant
	- (q11.3.1) $\det{A}=0$, if and only if, $\lambda=0$ is eigenvalue of $A$
	- Row Operations
		- If a multiple of one row of $A$ is **added** to another row to produce a matrix $B$, then $\det B=\det A$
		- If two rows of $A$ are **interchanged** to produce $B$, then $\det B=-\det A$
		- if one row of $A$ is **multiplied** by $k$ to produce $B$, then $\det B=k \cdot \det A$ 
	- (q4.3.3) $\det (tA)=t^n \det A$
	- $\det A$ is equal to the product of its eigenvalues (see q11.4.7)



> [!example]  Procedure: computing the detrminant
> 
> 1. convert $A$ into an upper triangular matrix $B$ via row operations of **switching rows**, and **adding multiplication of another row**. (but **NOT** scaling of row by scalar)
 > 	- Note: if during the row operations we find zero-row, then $\det A=0$
> 2. let $k$ be the number of times two rows are switched
> 3. $\det{A}=(−1)^kb_{11} · · · b_{nn}$

## Characteristic polynomial 
$$\det \left( \lambda I -A \right)$$
- (q11.4.6-7) finding coefficients of **the characteristic polynomial** of a matrix
	- The **free coefficient** of the characteristic polynomial of $A$ is $\det-A =(-1)^n\det{A}$
	- 

## Eigenvalues and Eigenvectors

- (d11.3.1) A nonzero column vector $v$ in $A$ that satisfies $Av=\lambda v$ for some scalar $\lambda$, is called an **eigenvector of** $A$, and $\lambda$ is the **eigenvalue associated with** $v$
- $\{ \mathbf{v}:(A-\lambda I) \mathbf{v}= \mathbf{0} \}$ is the **eigenspace of** $A$ **associated with its eigenvalue** $\lambda$. in other words, the set of all eigenvectors corresponding to eigenvalues $\lambda$, with the zero vector $\mathbf{0}$.

**Theorems**:
- (11.4.1) $\lambda$ is an eigenvalue of $A$, if and only if, $\lambda$ is a solution of the **characteristic equation** $\det(\lambda I-A)=0$
- similar matrices have the same eigenvalues (11.3.3), and the same algebraic multiplicities of eigenvalues ( #todo  )
- the sum of eigenvalues of $A$ equals to $\text{tr}A$ #todo 
- the multiplication of eigenvalues of $A$ equals to $\text{det}A$ #todo  
- the eigenvalues of diagonal matrix $\text{diag}{(\lambda_{1},\dots,\lambda_{{n}})}$, are $\lambda_{1},\dots,\lambda_{{n}}$   #todo 

>[!example] **Procedure**: Finding Eigenvalues and Eigenvectors
> 1. First, find the eigenvalues $\lambda$ of $A$ by solving the **characteristic equation** $\det \left( \lambda I -A \right) = 0$.
> 2. For each $\lambda$, find the basic eigenvectors $v \neq 0$ by finding the basic solutions to $\left( \lambda I - A \right) v = 0$.
> 
> To verify your work, make sure that $Av=\lambda v$ for each $\lambda$ and associated eigenvector $v$.

### Algebraic & geometric multiplicity

- (d11.5.2) The multiplicity of an eigenvalue $\lambda$ as a root of the characteristic equation is **the algebraic multiplicity** of $\lambda$ 
- (q11.5.2) The dimension of the eigenspace corresponding to $\lambda$ is called **the geometric multiplicity** of $\lambda$, which is $\dim{(\lambda I-A)}=n-\text{rank}(\lambda I-A)$     
- (11.5.3, q11.5.3)  $1\leq$ the **geometric multiplicity** $\leq$ the **algebraic multiplicity**
- finding the algebraic multiplicity of eigenvalue #todo 
- finding the geometric multiplicity of eigenvalue #todo 

### Whether a scalar is an eigenvalue of $A$

- (d11.3.1) the scalar $\lambda$ is called an **eigenvalue** of $A$, if there is a non-zero **column** vector $v$, such that: $Av=\lambda{v}$. (in such case, $v$ is called an **eigenvector** of $A$ that related to the eigenvalue $\lambda$.) 
- (q11.3.2a) if $\lambda$ is an eigenvalue of $A$, then for each $\mu$, $\mu\lambda$ is an eigenvalue of $\mu A$
- (q11.3.2b) if $\lambda$ is an eigenvalue of $A$, then , $\lambda^k$ is a eigenvalue of $A^k$. (for each natural $k$ )
- (11.4.1) $\lambda$ is an eigenvalue of $A$, if and only if, $\lambda$ is a solution of the **characteristic equation** $\det(\lambda I-A)$ is $0$
-  #todo - $\lambda$ is an eigenvalue of $A$, if and only if, the system of equations $(\lambda I-A)v=0$ has nontrivial solutions.

## Trace

- $\operatorname{tr}({A}) = \sum_{i=1}^n a_{ii} = a_{11} + a_{22} + \dots + a_{nn}$
- $\text{tr} A$ is the sum of its eigenvalues #todo 
- (10.7.6) $\text{tr}(AB)=\text{tr}(BA)$
- (10.7.5) similar matrices have the same trace
- $\text{tr}(A+B)=\text{tr}(A)+\text{tr}(B)$ 
- $\text{tr}(cA)=c\text{tr}(A)$ #todo 
- $\text{tr}(A)=\text{tr}(A^t)$ #todo 

## Similarity

- (d10.7.1) If $A$ and $B$ are square matrices, then we say that $A$ **is similar to** $B$ if there is an invertible matrix $M$ such that $A=M^{-1}BM$ 
- Similarity is an equivalence relation on the space of square matrices.
- (10.7.2) $A$ and $B$ square matrices of order $n$ on filed F are **similar**, if and only if, they represent the same linear transformation with respect to (possibly) different bases.
- #todo to show that two matrices are similar, show that are similar to the same diagonal matrix
- #todo let $A$ and $B$ are diagonalizable, and they both have the same eigenvalues, then they're similar (because similarity is transitive) 
- #todo let $A$ and $B$ are diagonalizable, and they both have the same characteristic polynomial, then they're similar (because similarity is transitive) 

shared properties: determinant (10.7.3), trace (10.7.5), eigenvalues (11.3.3), algebraic multiplicities of eigenvalues ( #todo  ),  characteristic polynomial (11.4.3)
	
## Diagonalizable

- (d11.3.4) if there exists an $n \times n$ invertible matrix $M$, such that $M^{-1}AM$ is a diagonal matrix, then $A$ is a **diagonalizable matrix**
- (d11.3.4) $A$ is diagonalizable, if and only if, $A$ is similar to a diagonal matrix
- (11.3.5) $T:V\to V$ is diagonalizable, if and only if, $A$ is diagonalizable
- (11.3.6) An $n \times n$ matrix with $n$ **distinct** eigenvalues is **diagonalizable**. 
- (11.3.7) $M$ is an $n \times n$ invertible matrix.  $M^{-1}AM$ is a diagonal matrix, (i.e. $A$ is diagonalizable), if and only if, the columns of $M$ are $n$ independent linearly eigenvectors of $A$. ^[in such case,  if the columns of $M$ are $v_{1},\dots,v_{n}$, and for each $i$ ($1\leq i\leq n$), $v_i$ is a eigenvector of $A$ that's related to the eigenvalue $\lambda_{i}$ , then $M^{-1}AM=\text{diag}{(\lambda_{1},\dots,\lambda_{{n}})}$]
- (q11.3.7) $A$ on a field $F$ is diagonalizable, if and only if, $F^n$ has a basis that consists of eigenvectors of $A$ 
- (q11.4.10) $A$ is diagonalizable, if and only if, $A^t$ is diagonalizable
- (11.5.4') The matrix $A$ is diagonalizable, if and only if, (i) the characteristic polynomial factors completely into linear factors and (ii) the algebraic multiplicity of each eigenvalue of $A$ is equal to its geometric multiplicity.
- #todo The matrix $A$ is diagonalizable, if and only if, the sum of the dimensions of the eigenspaces equals to $n$
- #todo $A^k=M{D}^{k}M^{-1}$, ($D$ is a diagonal matrix)


>[!example] Given a matrix $A$ which some of its values are $a$. For which value of $a$ is $A$ matrix diagonalizable?
> - Find the eigenvalues of $A$ using characteristic polynomial.
> - Find the values of $a$, for which the algebraic multiplicity of each eigenvalue $\lambda_{i}$ is equal to its geometric multiplicity which is $\dim{(\lambda_{i}I-A)}=n-\text{rank}(\lambda_{i}I-A)$.
> 

## Symmetric matrix

- (d3.2.6) ${A}\text{ is symmetric} \iff A=A^t$
- (q3.2.3) ${A}\text{ is symmetric} \implies {A}\text{ is square}$
- (q3.2.4) ${A}\text{ is diagonal} \implies {A}\text{ is symmetric}$
- (q3.2.4) sum of symmetric matries is symmetric matrix
- (q3.4.6) $A$ and $B$ are symmetric matries, then ${AB}\text{ is symmetric} \iff {AB=BA}$
- (q.4.3.10)  ${A}\text{ is anti-symmetric} \iff A^t=-A$
	- if $A_{n}$ is anti-symmetric, and $n$ is odd, then $\det A=0$ 

## Change of Basis matrix (Transition matrix) 
also *change-of-coordinates matrix*

**Definition:**
- (d8.4.6) Let $B=(v_{1},\dots ,v_{n})$ and $B'=(u_{1},\dots ,u_{n})$ bases of $V$. if $$\begin{align}
u_{1} &= a_{11}v_{1}+\dots+a_{n1}v_{n} \\ \vdots \notag \\ u_{n} &= a_{1n}v_{1}+\dots+a_{nn}v_{n}  \\ \end{align}$$then $$M=\begin{bmatrix} a_{11}  & \dots & a_{1n} \\    \vdots &  \ddots & \vdots \\ a_{n1}  & \dots & a_{nn} \end{bmatrix}$$ is the **transition matrix** from basis $B$ to basis $B'$. 
- the **transition matrix** from basis $B$ to basis $B'$ is the matrix that its columns are the coordinate vectors of the $B'$ vectors by $B$.

**Properties:**
- transition matrix is square matrix of $n$-order, which $n=\dim V$
- transition matrix is invertible matrix (by 8.4.5)

**Theorems:**
- (8.4.8) if $A$ is square matrix, and $[v]_{B}=A[v]_{B'}$ then $A$ is the transition matrix from $B$ to $B'$.  
- (8.4.8) if $M$ is the transition matrix from $B$ to $B'$, then $M^{-1}$ is the transition matrix from $B'$ to $B$
- (10.6.1) $T:V\to V$ and $B$ and $B'$ are bases of $V$. if $M$ transition matrix from $B$ to $B'$, then $[T]_{B'}=M^{-1}[T]_{B}M$. (or symmetrically $[T]_{B}=M[T]_{B'}M^{-1}$)
	- transition matrix from $B$ to $B'$ is $[I]^{B'}_{B}$, therefore $[T]_{B'}=[I]^{B}_{B'}[T]_{B}[I]^{B'}_{B}$

>[!example] Finding the transition matrix from an old basis to a new basis 
>1. Form the partitioned matrix $[\text{new basis} | \text {old basis}]$ in which the basis vectors (or coordinate vectors) are in column form. 
>2. Use elementary row operations to reduce the matrix in Step 1 to **RREF**.
>3. The resulting matrix will be $[{I} | \text{transition matrix from old to new}]$ where $I$ is an identity matrix.
>4. Extract the matrix on the right side of the matrix obtained in Step 3. 

### Transition matrix from a basis B to the standard basis

- if $B=(v_{1}, v_{2},\dots,v_{n})$, then $[v_{1}|v_{2}|\dots|v_{n}]$ is the transition matrix from $B$ to the standard basis


## Triangular matrix

- (4.3.8) if $A_{n}=[a_{ij}]$ is a triangular matrix, then $\det A=a_{11}a_{22} \cdots a_{nn}$


## Orthogonality

#todo Orthogonal matrix - This is not taught in the course.

