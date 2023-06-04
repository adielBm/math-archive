
# Matrix 

## Rank of Matrix $\rho{(A)}$

- (d8.5.4) the rank $\rho{(A)}$ is the dim. of the row/column space of $A$
- (q8.5.4) $\rho{(A)}=\rho{(A^n)}$
- (q8.5.5) $\rho{(A_{m \times n})}\leq\min{\{ m,n \}}$
- $\rho(A)$ is the number of the non-zero rows of row echelon form of $A$

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

# Dimension 

- (9.5.9) $V \cong W \iff \text{dim}{V}=\text{dim}{W}$ (on the same field, and infinite dim.)
- (9.6.1) $\text{dim}{(\text{Ker}{T})}+\text{dim}{(\text{Im}{T})}=\text{dim}{V}$. ($T:V\to W$ is lin. trans.)

### dimension of row/column space of matrix (the rank)

- find the number non-zero rows of the row echelon form of the matrix 

### dimension of solution sub-space of homogeneous system

- Theorem 8.6.1 - $A\textbf{x}=\textbf{0}$, ($n$ variables, and $P$ is the solutions sub-space), then $\dim{P}=n-\rho{(A)}$

# Coordinate vector

> q8.4.1b (matrices space), q8.4.2b (polynomial space)

# Linear Transformation

## image of linear transformation

- (9.3.6) let $\{ v_{1},\dots ,v_{n} \}$ spans $V$, then $\text{Im}{T}=\text{Sp}{(\{ T(v_{1}),\dots,T(v_{n}) \})}$

>q9.3.2c, q9.3.3, q9.4.2

>for Im of indep. subset of V (lin. trans. that is **one-to-one**). see 9.5.6 

## kernel of linear transformation

- $\ker(T) = \{ v \in V : T(v) = 0_W\}$

## linear transformation so that..

- linear transformation $T:V\to W$ s.t. $A=\{ v_{1},\dots ,v_{k} \}$ spans $\text{Ker{(T)}}$
	- find basis to $\text{Ker{(T)}}$
	- take the found basis, and extend it to basis of $F^n$
	- set the Im of the basis 
	- 

### properties of linear transformation

#### injective $\iff$ surjective $\iff$ isomorphism

- (9.6.2) for $V,W$ with the same dim., there is equivalence between injective, surjective and isomorphism of $T:V\to W$
