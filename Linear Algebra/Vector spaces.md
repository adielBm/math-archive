# Spaces 

### Two spaces are equal, $U=V$

- Option 1: check if $U=\text{Sp}{(S)}$ is equel to $V=\text{Sp}{(T)}$
	- check if the matrix by S as rows, is ***row-equivalent*** to the matrix by T as rows (7.5.12)
- Option 2: if $U\subseteq V$ then $U=V \iff \dim V=\dim U$. (8.3.4)

### Two vector spaces are isomorphic, $V\cong{W}$

assumption: the spaces are on the same filed $F$  

- (9.5.7, 9.5.9) $\dim{V}=\dim{W} \iff V\cong{W}$
- (9.5.8) $\dim{V}=n\implies V\cong{F^n}$


# Dimension 

- (9.5.9) $V \cong W \iff \text{dim}{V}=\text{dim}{W}$ (on the same field, and infinite dim.)
- (9.6.1) $\text{dim}{(\text{Ker}{T})}+\text{dim}{(\text{Im}{T})}=\text{dim}{V}$. ($T:V\to W$ is lin. trans.)

### dimension of row/column space of a matrix

>see [[#Rank of Matrix $ rho{(A)}$]] 

### dimension of solution sub-space of homogeneous system

- (8.6.1) -let $A\textbf{x}=\textbf{0}$, ($n$ variables, and $P$ is the solutions sub-space), then $\dim{(P)}=n-\rho{(A)}$
- this dim is called also nullity of A, or $\text{nul}{(A)}$


# Linear independence

## whether a set of vectors $K=\set{{v}_1,\dots,{v}_k}$, is a linearly independent

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


# Span

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

- the basis of **the row space** of a matrix $B^t$, is the basis of **the column space** of a matrix $B$

### basis of the sub-space $U=\text{Sp}({\set{v_{1},v_{2},\dots,v_{k}   }})$ of ${F}^n$
reducing a span set to a basis by removing a vectors 
(q8.5.2b)

- set the ${\set{v_{1},v_{2},\dots,v_{k}   }}$ as row vecor of matrix, and then follow [[#basis of the row space of a matrix $B$]] 

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

### Extending a linearly independent set to a basis by adding a vectors

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

- coordinate vector of image (10.2.1) - $[T(v)]_{C}=[T]^{B}_{C}[v]_{B}$







___







