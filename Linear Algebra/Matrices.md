$\large A$ is $m\times n$ matrix 

## Arithmetic 

### Matrix addition & multiplication 

**Definitions:**
- Matrix addition - $A+B=C$ where $a_{ij}+b_{ij}=c_{ij}$
- Matrix multiplication - $A_{m\times n}B_{n\times p}=C_{m \times p}=[c_{ij}]$, where $c_{ij}$ is the dot product of the $i$th row of $A$ and the $j$th column of $B$ 

**Properties:**
- **Commutative (addition)** $A+B=B+A$
- **Commutative (multiplication)** see [[#Commuting]]
- **Associative (addition)** $A+(B+C)=(A+B)+C$
- **Associative (multiplication)** $A(BC)=(AB)C$
- **distributive (left)** $A(B+C)=AB+AC$
- **distributive (right)** $(B+C)A=BA+CA$

###  Matrix–Vector Product

- $(A+B)\mathbf{v}=A\mathbf{v}+B\mathbf{v}$
- $A(\mathbf{u}+\mathbf{v})=A\mathbf{u}+A\mathbf{v}$
- $A(c\mathbf{u})=c(A\mathbf{u})$

- $A\mathbf{u}=A\mathbf{v}\iff A(\mathbf{u}-\mathbf{v})=0$

## Row Echelon form (REF)

- (1.11.1) $\text{REF}(A)$ is row equivalence to $\text{RREF}(A)$
- (8.5.1) The nonzero rows of $\text{REF}(A)$ are a basis for $\text{row-space(A)}$.

### Reduced Row Echelon form (RREF)

- **Uniqueness:** Each matrix is row equivalent to one and only one reduced echelon matrix. 

## Row equivalence

Row equivalence is an *equivalence relation*

**Definitions:** - The following statements are **equivalent**:
- $A$ and $B$ are row equivalent
- it is possible to transform $A$ into $B$ by a sequence of elementary row operations
- $\text{row-space}(A)=\text{row-space}(B)$
- $\text{null}(A)=\text{null}(B)$
- There exists an invertible matrix $P$ such that $A=PB$.

**Properties:**
If $A$ and $B$ are row equivalent matrices, then: 
- (q7.5.12) $\text{row-space}(A)=\text{row-space}(B)$
- A given set of column vectors of $A$ is linearly independent if and only if the corresponding column vectors of $B$ are linearly independent. 
- A given set of column vectors of $A$ forms a basis for the column space of $A$ if and only if the corresponding column vectors of $B$ form a basis for the column space of $B$. 
- $A$ and $B$ have the same rank

## Rank

**Notation**: $\text{rank}{(A)}=\rho{(A)}$

**Definitions:**
- (d8.5.4) $\rho{(A)}=\dim(\text{row-space(A)})=\dim(\text{column-space(A)})$
- $\rho(A)$ is the maximal number of linearly independent **rows**
- $\rho(A)$ is the maximal number of linearly independent **columns**
- $\rho(A)=\dim(\text{Im}(T_{A}))$
- $\rho(A)=n-\dim(\text{null}{(A)})$
- $\rho(A)$ is the number of the non-zero rows of $\text{REF}(A)$
- $\rho(A)$ is the number of pivots in $\text{RREF}(A)$

**Theorems:**
- (q8.5.4) $\rho{(A)}=\rho{(A^t)}$
- (q8.5.5) $\rho{(A_{m \times n})}\leq\min{\{ m,n \}}$
	- if $\rho{(A)}=\min{\{ m,n \}}$ then $A$ has **full rank**.
		- if $\rho{(A)}=n$ then $A$ has **full column rank**. ($f(\mathbf{x})=A\mathbf{x}$ is injective)
		- if $\rho{(A)}=m$ then $A$ has **full row rank**. ($f(\mathbf{x})=A\mathbf{x}$ is surjective) (A's rows are linearly indepndent #todo )
	- Otherwise if $\rho{(A)}<\min{\{ m,n \}}$, then $A$ has **rank deficient**. 
- (q8.5.6) $\rho{(AB)}\leq\min{\{ \rho{(A)}, \rho{(B)} \}}$
- (q8.5.7a) let $A_{m \times n}$, and $B_{n}$ invertible matrix, then $\rho(AB)=\rho(A)$ 
- (q8.5.7b) let $A_{m \times n}$, and $B_{m}$ invertible matrix, then $\rho(BA)=\rho(A)$ 
- (8.6.1) **Rank–nullity** theorem  $\rho(A)+\dim(\text{nul}{(A)})=n$
- $A=0\iff \rho(A)=0$. #todo 
- Row equivalent matrices have the same rank #todo 
- rank of **square matrix:**
	- (q8.5.8a) let $A$ square matrix of order $n$, then $\rho(A)=n \iff |A|\neq 0$  
	- (q10.5.3) $A,B$ are square matrices of order $n$, then $\rho{(AB)}\geq \rho(A)+\rho(B)-n$

## Nullity 

- (8.6.1) $\mathrm{nullity}(A)=\dim{\mathrm{(null(A))}}=n-\rho({A})$

## Transformation matrix

Matrix Representations of Linear Transformation

- (d10.1.1) $T:V\to W$, and $B=(v_{1},\dots,v_{n})$ and $C=(w_{1},\dots,w_{n})$ are bases of $V$ and $W$. (respectively) 
$$[T]_{C}^{B}=\left[\begin{array}{ccc} | & & | \\ [T({v_{1}})]_{C} & \cdots & [T( {v_{n}})]_{C} \\ | & & | \end{array} \right]_{m\times n}$$


## Transpose

- Notation: $A^t$, $A^\top$
- (3.2.4)  $(A^t)^t=A$
- $(A+B)^t=A^t+B^t$
- (3.4.5) $(AB)^t=B^tA^t$
- $(cA)^{t}=cA^{t}$

## Equivalence

>[!warning] This term is beyond the scope of the course. 

Matrix equivalence is an equivalence relation on the space of rectangular matrices.

Two $m\times n$ matrices $A$ and $A'$ are called **equivalent** if $$A'=P^{-1}AQ$$for some $n\times n$ matrix $Q$ and $m\times m$ matrix $P$.

Equivalent matrices represent the same linear transformation $T:V\to{W}$ under two different choices of a pair of bases of $V$ and $W$, with $Q$ and $P$ being the change of basis matrices in $V$ and $W$ respectively.

- $B,C$ are **old bases** of $V,W$ (respectively)
- $B',C'$ are **new bases** of $V,W$ (respectively)
- $Q$ is change-of-basis $n\times n$ invertible matrix of $V$ from $B$ to $B'$
- $P$ is change-of-basis $m\times m$ invertible matrix of $W$ from $C$ to $C'$
- $A=[T]^{B}_{C}$ is the transformation matrix by the **old bases**
- $A'=[T]^{B'}_{C'}$ is the transformation matrix by the **new bases**


## Theorems 

- The following statements are **equivalent**:
	- For each $\mathbf{b}$ in $\mathbb{R}^m$, the equation $A\mathbf{x}=\mathbf{b}$ has a solution
	- Each $\mathbf{b}$ in $\mathbb{R}^m$ is a linear combination of the columns of $A$
	- The columns of $A$ span $\mathbb{R}^m$
	- $A$ has a pivot postion in every row

- The following statements are **equivalent**:
	- The equation $A\mathbf{x}=\mathbf{b}$ has a unique least-squares for each $\mathbf{b}$ in $\mathbb{R}^m$
	- The columns of $A$ are linearly indepndent
	- The matrix $A^tA$ is invertible 

- $AB=0\iff \text{column-space}(B)\subseteq{\text{null}(A)}$


# Square Matrices

Let $A$ be an $n \times n$ square matrix.

## Invertibility 

- **Theorem 3.10.6**: Let $A$ be a $n$-ordered square matrix over a field $F$. The following statements are **equivalent**:
	- $A$ is an **invertible matrix**
	- $A$ can be expressed as a finite product of elementary matrices.
	- There exists a $B$ such that $BA=I$
	- There exists a $B$ such that $AB=I$
	- There exists a $B$ such that $AB=BA=I$, (in such case $A^{-1}=B$, and $B^{-1}=A$) ()
	- $A$ is row-equivalent to $I$.
	- $A$ is column-equivalent to $I$.
	- $\text{RREF}(A)=I$
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
	- (10.5.1, and 9.6.2) $\text{null}(A)=\{ 0 \}$
	- $(\text{null}(A))^{\perp}=F^n$
	- $\dim{(\text{null}(A))=0}$
	- The linear transformation mapping $\mathbf{x}$ to $A\mathbf{x}$ is **surjective**; that is, the equation $A\mathbf{x}=\mathbf{b}$ has at least one solution for each $\mathbf{b}$ in $F^n$.
	- The linear transformation mapping $\mathbf{x}$ to $A\mathbf{x}$ is **injective**; that is, the equation $A\mathbf{x}=\mathbf{b}$ has at most one solution for each $\mathbf{b}$ in $F^n$.
	- The linear transformation mapping $\mathbf{x}$ to $A\mathbf{x}$ is **bijective**; that is, the equation $A\mathbf{x}=\mathbf{b}$ has exactly one solution for each $\mathbf{b}$ in $F^n$. ($A\mathbf{x}=\mathbf{b}\implies \mathbf{x}=A^{-1}\mathbf{b}$
	- $A\mathbf{x}=\mathbf{0}\implies \mathbf{x}=\mathbf{0}$

**Properties:**
- (3.8.3) if $A$ is invertible, then:
	- (left-cancellable) $AB=AC\implies B=C$ 
	- (right-cancellable) $BA=CA\implies B=C$
- (3.8.4c) if $A,B$ are invertible (the same order), then $AB$ is also invertible. (in such case $(AB)^{-1}=B^{-1}A^{-1}$) 
- (3.8.4d) if $A$ is invertible, and $s\neq 0$, then $sA$ is also invertible. (in such case $(sA)^{-1}=\frac{1}{s}A^{-1}$)
- if $A$ and $B$ are invertible, then they are row equivalent

**Theorems:**
- (4.5.2) $A,B$ are square matries, and $AB=I$, then:
	- $A$ and $B$ are both invetible
	- $A^{-1}=B$
	- $B^{-1}=A$
	- $AB=BA=I$
- 

> [!example] **Procedure:** determine whether a square matrix $A$ is invertible and, if so, find $A^{−1}$: 
>	- Form the augmented matrix $[A | I_{n}]$ and put it into RREF. 
>	- If the RREF has the form $[I_{n} | B]$, then $A$ is invertible and $B=A^{−1}$. 
>	- else, if the matrix in the left half of the RREF is not $I_{n}$, then $A$ is singular. 

> **WolframAlpha** `inverse [matrix]`

## Elementary matrix

- $A$ is called an **elementary matrix** if it can be obtained from an identity matrix by performing a single elementary row operation. 
- Every elementary matrix is invertible, and the inverse is also an elementary matrix. 

## Determinant 

- **Notation:** $\det A=|A|$ 

- **Cofactor Expansion**: $\det(A)=\sum^{n}_{j=1}(-1)^{i+j}a_{ij}\det(A_{{ij}})$
	- $a_{ij}$ is the entry of the $i$th row and jth column of $A$
	- $A_{ij}$ is the submatrix obtained by removing the $i$th row and the $j$th column of $A$
	- Here $j$ is variable and $i$ is some consonent, but the opposite is also possible.
	- $M_{ij}=\det(A_{{ij}})$ is $i,j$ **minor** of $A$.
	- $C_{ij}=(-1)^{i+j}M_{ij}$ is **cofactor** of entry $a_{ij}$
 
- **Theorems:**
	- (4.5.1) $\det (AB)=\det (A) \det (B)$
	- (4.3.1) $\det (A)=\det(A^t)$
	- (4.3.5) if $A$ has two equal rows (or colmuns), then $\det A=0$
	- (4.4.1) $\det{A}\neq0 \iff A\text{ is invertible}$
	- (4.3.8) if $A_{n}=[a_{ij}]$ is a triangular matrix, then $\det A=a_{11}a_{22} \cdots a_{nn}$
	- (10.7.3) **similar matrices** have the same determinant
	- (q11.3.1) $\det{A}=0$, if and only if, $\lambda=0$ is eigenvalue of $A$
	- Row Operations
		- If a multiple of one row of $A$ is **added** to another row to produce a matrix $B$, then $\det B=\det A$
		- If two rows of $A$ are **interchanged** to produce $B$, then $\det B=-\det A$
		- if one row of $A$ is **multiplied** by $k$ to produce $B$, then $\det B=k \cdot \det A$ 
	- (q4.3.3) **Homogeneity:** $\det (tA)=t^n \det A$
	- $\det A$ is equal to the product of its eigenvalues (see q11.4.7)


> [!example]  Procedure: computing the detrminant
> 
> 1. convert $A$ into an upper triangular matrix $B$ via row operations of **switching rows**, and **adding multiplication of another row**. (but **NOT** scaling of row by scalar)
 > 	- Note: if during the row operations we find zero-row, then $\det A=0$
> 2. let $k$ be the number of times two rows are switched
> 3. $\det{A}=(−1)^kb_{11} · · · b_{nn}$

## Trace

- $\operatorname{tr}({A}) = \sum_{i=1}^n a_{ii} = a_{11} + a_{22} + \dots + a_{nn}$
- $\text{tr} A$ is the sum of its eigenvalues #todo 
- (10.7.6) $\text{tr}(AB)=\text{tr}(BA)$
- (10.7.5) similar matrices have the same trace
- $\text{tr}(A+B)=\text{tr}(A)+\text{tr}(B)$ 
- $\text{tr}(cA)=c\text{tr}(A)$ #todo 
- $\text{tr}(A)=\text{tr}(A^t)$ #todo 

## Characteristic polynomial 
$$p_{A}=\det \left( \lambda I -A \right)$$
**Properties:**
- The **coefficient of** $\lambda^{n}$ is $1$
- (q11.4.6) The **coefficient of** $\lambda^{n-1}$ equals $\text{tr}(-A)=-\text{tr}(A)$ 
- (q11.4.7) The **free coefficient** equals $\det(-A) =(-1)^n\det{(A)}$

## Eigenvalues

Definitions of **eigenvalue**. The following statements are **equivalent**:
-  $\lambda$ is an **eigenvalue** of $A$
- (d11.3.1) There is a **non-zero** vector $v$ such that $Av=\lambda{v}$. (in such case, $v$ is called an **eigenvector** of $A$ that related to the eigenvalue $\lambda$) 
- $(A-\lambda I)$ is singular
- $\text{rank}(A-\lambda I)<n$
- $(\lambda I-A)v=0$ has nontrivial solutions, i.e. $\text{null}(\lambda I-A)\neq \{ 0 \}$
- (11.4.1) The **characteristic equation** $\det(\lambda I-A)=0$
- $\lambda$ is a root of the characteristic equation $\det(xI-A)=0$

**Theorems**:
- Similar matrices have the same eigenvalues (11.3.3), the same **characteristic polynomial** (11.4.3), and the same algebraic multiplicities of eigenvalues ( #todo  ) 
- The sum of eigenvalues of $A$ equals to $\text{tr}A$ #todo 
- The product of eigenvalues of $A$ equals to $\text{det}A$ #todo  
- The eigenvalues of diagonal matrix $\text{diag}{(\lambda_{1},\dots,\lambda_{{n}})}$, are $\lambda_{1},\dots,\lambda_{{n}}$   #todo 
- (q11.3.2a) if $\lambda$ is an eigenvalue of $A$, then for each $\mu$, $\mu\lambda$ is an eigenvalue of $\mu A$
- (q11.3.2b) if $\lambda$ is an eigenvalue of $A$, then , $\lambda^k$ is a eigenvalue of $A^k$. (for each natural $k$ )

### Eigenvectors 

Definitions of **eigenvector**. The following statements are **equivalent**:
- $v$ is an **eigenvector** of $A$ that related to $\lambda$
- (d11.3.1) $v$ is nonzero vector in $\mathbb{R}^n$ such that $Av=\lambda v$

### Eigenspace 

Definitions of the **eigenspace of** $A$ **associated with its eigenvalue** $\lambda$.
- $\{ \mathbf{v}\mid(A-\lambda I) \mathbf{v}= \mathbf{0} \}$
- $\{ \mathbf{v}\mid A\mathbf{v}=\lambda \mathbf{v} \}$
- $\{ \text{eigenvectors corresponding to } \lambda \}\cup \{ \mathbf{0} \}$
- $\text{null}(\lambda I-A)$

### Algebraic & geometric multiplicity

- (d11.5.2) The **algebraic multiplicity** of $\lambda$ is the multiplicity of an eigenvalue $\lambda$ as a root of the characteristic equation.
- (q11.5.2) The **geometric multiplicity** of $\lambda$, is the dimension of the eigenspace corresponding to $\lambda$, which is $\dim{(\lambda I-A)}=n-\text{rank}(\lambda I-A)$     

- (11.5.3, q11.5.3)  $1\leq$ the **geometric multiplicity** $\leq$ the **algebraic multiplicity**

- finding the algebraic multiplicity of eigenvalue #todo 
- finding the geometric multiplicity of eigenvalue #todo 


>[!example] **Procedure**: Finding Eigenvalues and Eigenvectors
> 1. First, find the eigenvalues $\lambda$ of $A$ by solving the **characteristic equation** $\det \left( \lambda I -A \right) = 0$.
> 2. For each $\lambda$, find the basic eigenvectors $v \neq 0$ by finding the basic solutions to $\left( \lambda I - A \right) v = 0$.
> 
> To verify your work, make sure that $Av=\lambda v$ for each $\lambda$ and associated eigenvector $v$.


## Similarity

Similarity is an *equivalence relation* on the space of square matrices.

$A$ and $B$ are square matrices

Definitions of **similarity**. The following statements are **equivalent**:
- $A$ and $B$ are similar
- (d10.7.1) There is an invertible matrix $P$ such that $A=P^{-1}BP$ 
- (10.7.2) $A$ and $B$ represent **the same linear transformation**. (possibly different bases)

**Theorems:**
- #todo to show that two matrices are similar, show that are similar to the same diagonal matrix
- #todo let $A$ and $B$ are diagonalizable, and they both have the same eigenvalues, then they're similar (because similarity is transitive) 
- #todo let $A$ and $B$ are diagonalizable, and they both have the same characteristic polynomial, then they're similar (because similarity is transitive) 

**Properties:**
- If the matrices $A$ and $B$ are similar, then
	- $A=I\iff B=I$ #todo 
	- $A=0\iff B=0$ #todo 
	- $A$ is **invertible**, if and only if $B$ is also **invertible** #todo 
	- $\det(A)=\det(B)$ (10.7.3)
	- $\text{tr}(A)=\text{tr}(B)$ (10.7.5)
	- $A$ and $B$ have the same **eigenvalues** (11.3.3)
	- $A$ and $B$ have the same **algebraic multiplicities** of eigenvalues #todo 
	- $A$ and $B$ have the same **characteristic polynomial** (11.4.3)
	- $\dim(\text{null}(A))=\dim(\text{null}(B))$
	- $\text{rank}(A)=\text{rank}(B)$

## Triangular matrix


**Properties:**
-  if $A_{n}=[a_{ij}]$ is a triangular matrix, then
	- $\det A=a_{11}a_{22} \cdots a_{nn}$ (4.3.8)
	- the eigenvalues of $A$ are $a_{11},a_{22},\dots,a_{nn}$ 
		- each eigenvalue occurs exactly k times on the diagonal, where k is its algebraic multiplicity
	- the characteristic polynomial of $A$ is $p_{A}=(x-a_{11})(x-a_{22})\cdots(x-a_{nn})$
	- 

## Diagonal matrix

- **Addition:** $\text{diag}{(a_{1},\dots ,a_{n})}+\text{diag}{(b_{1},\dots ,b_{n})}=\text{diag}{(a_{1}+b_{1},\dots ,a_{n}+b_{n})}$
- **Multiplication** $\text{diag}{(a_{1},\dots ,a_{n})}\text{diag}{(b_{1},\dots ,b_{n})}=\text{diag}{(a_{1}b_{1},\dots ,a_{n}b_{n})}$
- Powers of a matrix  $(\text{diag}{(a_{1},\dots,a_{{n}})})^k=\text{diag}{(a_{1}^k,\dots,a_{n}^k)}$
- $\text{diag}{(a_{1},\dots ,a_{n})}\text{ is invertible}\iff a_{1},\dots,a_{n}\neq 0$. in such case $\text{diag}{(a_{1},\dots ,a_{n})^{-1}}=\text{diag}{(a_{1}^{-1},\dots ,a_{n}^{-1})}$
- A matrix is diagonal, if and only if, it is both *upper-* and *lower-triangular*.
- A diagonal matrix is symmetric.
- $\det(\text{diag}{(a_{1},\dots ,a_{n})})=a_{1}\cdots a_{n}$

## Diagonalizable

- Diagonalizable definition. The following statements are equivalent. 
	- $A$ is a **diagonalizable matrix**
	- (d11.3.4) There exists an $n \times n$ invertible matrix $P$, such that $P^{-1}AP$ is a diagonal matrix
	- (d11.3.4) $A$ is similar to a diagonal matrix
	- (11.3.7) $A$ has $n$ linearly independent eigenvectors. (they are $P$'s columns. that are $v_{1},\dots,v_{n}$, and $v_i$ is a **eigenvector** of $A$ that's related to the **eigenvalue** $\lambda_{i}$. and $P^{-1}AP=\text{diag}{(\lambda_{1},\dots,\lambda_{{n}})}$ )
	- (q11.3.7) $F^n$ has a basis that consists of eigenvectors of $A$ 
	- (11.3.5) $T_{A}:V\to V$ is diagonalizable
	- (q11.4.10) $A^t$ is diagonalizable
	- (11.5.4') 
		- (i) the characteristic polynomial factors completely into linear factors. and 
		- (ii) the geometric multiplicity of every eigenvalue is equal to the algebraic multiplicity
	- #todo The sum of the dimensions of the eigenspaces equals to $n$


- (11.3.6) if $A$ has $n$ **distinct** eigenvalues, then $A$ diagonalizable
- #todo $A^k=P{D}^{k}P^{-1}$, ($D$ is a diagonal matrix)



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

- (d8.4.6) Let $B=(v_{1},\dots ,v_{n})$ and $C=(u_{1},\dots ,u_{n})$ bases of $V$. if $$\begin{align}
u_{1} &= a_{11}v_{1}+\dots+a_{n1}v_{n} \\ \vdots \notag \\ u_{n} &= a_{1n}v_{1}+\dots+a_{nn}v_{n}  \\ \end{align}$$then $$P=\begin{bmatrix} a_{11}  & \dots & a_{1n} \\    \vdots &  \ddots & \vdots \\ a_{n1}  & \dots & a_{nn} \end{bmatrix}=\left[\begin{array}{ccc} | & & | \\ [{u_{1}}]_{B} & \cdots & [{u_{n}}]_{B} \\ | & & | \end{array} \right]$$ is the **transition matrix** from basis $B$ to basis $C$. 
- the **transition matrix** from basis $B$ to basis $C$ is the matrix that its columns are the coordinate vectors of the $C$ vectors by $B$.
- $\forall{v}\in{V} :P[v]_{C}=[v]_{B}, \quad [v]_{C}=P^{-1}[v]_{B}$
- (8.4.9) $P^{-1}$ is the transition matrix from $C$ to $B$
- Transition matrix is square matrix of $n$-order, where $n=\dim V$
- (by 8.4.5) Transition matrix is invertible matrix 

**Theorems:**
- (8.4.8) if $A$ is square matrix, and $[v]_{B}=P[v]_{C}$ for each $v\in{V}$, then $P$ is the transition matrix from $B$ to $C$. 
- (10.6.1) $T:V\to V$ and $B$ and $C$ are bases of $V$. if $P$ transition matrix from $B$ to $C$, then $[T]_{C}=P^{-1}[T]_{B}P$. (or symmetrically $[T]_{B}=P[T]_{C}P^{-1}$)
	- transition matrix from $B$ to $C$ is $[I]^{C}_{B}$, therefore $[T]_{C}=[I]^{B}_{C}[T]_{B}[I]^{C}_{B}$

>[!example] Finding the transition matrix from an old basis to a new basis 
>1. Form the partitioned matrix $[\text{new basis} | \text {old basis}]$ in which the basis vectors (or coordinate vectors) are in column form. 
>2. Use elementary row operations to reduce the matrix in Step 1 to **RREF**.
>3. The resulting matrix will be $[{I} | \text{transition matrix from old to new}]$ where $I$ is an identity matrix.
>4. Extract the matrix on the right side of the matrix obtained in Step 3. 

### Transition matrix from a basis B to the standard basis

- if $B=(v_{1}, v_{2},\dots,v_{n})$, then $[v_{1}|v_{2}|\dots|v_{n}]$ is the transition matrix from $B$ to the standard basis

## Orthogonality

#todo Orthogonal matrix - This is not taught in the course.
## Commuting

- (d3.6.2) $A$ and $B$ are said to commute if $AB=BA$
- (3.6.3) $(tI)A=A(tI)$
- $A$ and $B$ share the same $n$ independent eigenvectors if and only if $AB=BA$.
