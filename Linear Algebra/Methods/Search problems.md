# Linear Systems

## Solving Linear Systems 

- Gaussian elimination (REF)
- Gauss–Jordan elimination (RREF)
- If $A$ is an invertible $n×n$ matrix, then for every $n×1$ matrix $\textbf{b}$, the system of equations $A\textbf{x}=\textbf{b}$ has exactly one solution, namely, $\textbf{x}=A^{−1}\textbf{b}$ 
- (4.6.1) Cramer's rule 

# Matrix 

## Rank of Matrix $\rho{(A)}$

Defintions:
- (d8.5.4) the rank $\rho{(A)}$ is the dim. of the row/column space of $A$
- $\rho(A)$ is the number of the non-zero rows of row echelon form of $A$
- $\rho(A)$ is the number of pivots in the RREF of $A$. 

Properties:
- (q8.5.4) $\rho{(A)}=\rho{(A^n)}$
- (q8.5.5) $\rho{(A_{m \times n})}\leq\min{\{ m,n \}}$
- (q10.5.3) $A,B$ are square matries of order $n$, then $\rho{(AB)}\geq \rho(A)+\rho(B)-n$

## Determinant $|A|$

- **Procedure:** 
	1. convert $A$ into an upper triangular matrix $B$ via row operations of **switching rows**, and **adding multiplication of another row**. (but **NOT** scaling of row by scalar)
		- Note: if during the row operations we find zero-row, then $\det A=0$
	2. let $k$ be the number of times two rows are switched
	3. $\det{A}=(−1)^kb_{11} · · · b_{nn}$
- **Theormes:**
	- (10.7.3) **similar matrices** have the same determinant

## Inversion matrix $A^{-1}$

let A square matrix, find $A^{-1}$, see [[Decision problems#Invertibility]]

> **WolframAlpha** `inverse [matrix]`

## Transition matrix

thorems 
- ()

### process  
1. Form the partitioned matrix $[\text{new basis} | \text {old basis}]$ in which the basis vectors (or coordinate vectors) are in column form. 
2. Use elementary row operations to reduce the matrix in Step 1 to **RREF**.
3. The resulting matrix will be $[{I} | \text{transition matrix from old to new}]$ where $I$ is an identity matrix.
4. Extract the matrix on the right side of the matrix obtained in Step 3. 

### transition matrix from a basis B to the standard basis

- if $B=(v_{1}, v_{2},\dots,v_{n})$, then $[v_{1}|v_{2}|\dots|v_{n}]$ is the transition matrix from B to the standard basis

# Basis

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

- the basis of **the row space** of a matrix $B^t$, is the basis of **the column space** of a matrix $B$

### basis of the sub-space $U=\text{Sp}({\set{v_{1},v_{2},\dots,v_{k}   }})$ of ${F}^n$
reducing a span set to a basis by removing a vectors 
(q8.5.2b)

- set the ${\set{v_{1},v_{2},\dots,v_{k}   }}$ as row vecor of matrix, and then follow [[#basis of the row space of a matrix $B$]] 

###### OR:

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

### Extending a linearly independent set to a basis by adding a vectors

#todo 
- Obtain the reduced row echelon form (RREF) of the matrix as row of vectors. and then complete it to identity matrix. (the rows for the complete are the vectors for complete to basis)
- q8.3.6
- q8.6.4 



### basis for ImT

### basis for KerT



# Dimension 

- (9.5.9) $V \cong W \iff \text{dim}{V}=\text{dim}{W}$ (on the same field, and infinite dim.)
- (9.6.1) $\text{dim}{(\text{Ker}{T})}+\text{dim}{(\text{Im}{T})}=\text{dim}{V}$. ($T:V\to W$ is lin. trans.)

### dimension of row/column space of a matrix

>see [[#Rank of Matrix $ rho{(A)}$]] 

### dimension of solution sub-space of homogeneous system

- (8.6.1) -let $A\textbf{x}=\textbf{0}$, ($n$ variables, and $P$ is the solutions sub-space), then $\dim{(P)}=n-\rho{(A)}$
- this dim is called also nullity of A, or $\text{nul}{(A)}$

# Coordinate vector

> q8.4.1b (matrices space), q8.4.2b (polynomial space)

- coordinate vector of image (10.2.1) - $[T(v)]_{C}=[T]^{B}_{C}[v]_{B}$

# Linear Transformation

## Image of linear transformation $\text{Im}T$

- (9.3.6) let $T:V\to W$, and $\text{Sp}\{ v_{1},\dots ,v_{n} \}=V$, then, $\text{Im}{T}=\text{Sp}{(\{ T(v_{1}),\dots,T(v_{n}) \})}$
- (9.3.7) let $A_{m \times n}$ matrix on field $F$, and $T:F^n\to F^m$, where $T_{A}(v)=Av$, then, $\text{Im}(T_{A})=\text{Col}{(A)}$ (the colmun space of $A$)
- (9.6.2) if $T:V\to W$ is isomorphism from $V$ to $W$, and the dimV=dimW, then $\text{Im}{T}=W$

>q9.3.2c, q9.3.3, q9.4.2

>for Im of indep. subset of V (lin. trans. that is **one-to-one**). see 9.5.6 

## kernel of linear transformation $\text{Ker}T$

- $\ker(T) = \{ v \in V : T(v) = 0_W\}$

>see 9.6.2 

## linear transformation so that..

- linear transformation $T:V\to W$ s.t. $A=\{ v_{1},\dots ,v_{k} \}$ spans $\text{Ker{(T)}}$
	- find basis to $\text{Ker{(T)}}$
	- take the found basis, and extend it to basis of $F^n$
	- set the Im of the basis 
	- 
	

## Matrix for a Linear Transformation 

$T:V\to W$, and $B=(v_{1},\dots,v_{n})$ and $C=(w_{1},\dots,w_{n})$ are basises of $V$ and $W$. (respectively) 
$$[T]_{C}^{B}=\left[\begin{array}{ccc} | & & | \\ [T({v_{1}})]_{C} & \cdots & [T( {v_{n}})]_{C} \\ | & & | \end{array} \right]_{m\times n}$$

## Finding $T(v)$ Indirectly 

1. Compute the coordinate vector $[v]_{B}$
2. Compute $[T(v)]_{C}=[T]_{C}^{B}[v]_{B}$
3. Reconstruct $T(v)$ from its coordinate vector $[T(v)]_{C}$

