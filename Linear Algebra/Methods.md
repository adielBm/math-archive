# Search problems 

## Basis

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
- q8.3.6
- q8.6.4 

## Dimension 

### dimension of row/column space of matrix (the rank)

- find the number non-zero rows of the row echelon form of the matrix 

### dimension of solution sub-space of homogeneous system

- Theorem 8.6.1 - $A\textbf{x}=\textbf{0}$, ($n$ variables, and $P$ is the solutions sub-space), then $\dim{P}=n-\rho{(A)}$

## Coordinate vector

> q8.4.1b (matrices space), q8.4.2b (polynomial space)


# Decision problems

## Linear systems

### Linear systems consistent

- Rouché–Capelli theorem (8.6.2) - A system of linear equations with $n$ variables has a solution if and only if the rank of its coefficient matrix $A$ is equal to the rank of its augmented matrix $[A|b]$. That is $\rho([A|B])=\rho(A)$

## Linear independence

### Set of vectors $K=\set{{v}_1,\dots,{v}_k}$, is a linearly independent
- by the defintion, $K$ is linearly independent, if  $\lambda_1{v}_1 + \lambda_2{v}_2 + \cdots + \lambda_k{v}_k = {0}\implies{\lambda_{1},\dots,{\lambda_{k}}}=0$.
- in other words, check if the linear sys. has the only the trivial solution.

> q8.4.1a (matrices space), q8.4.2a (polynomial space)

####  Set of matrices, is linearly in/dependent
- q8.2.5 (is dependent)
- q8.4.1a (is independent)

## Spaces 

### Two spaces are equal $U=V$

- Option 1: if $U\subseteq V$ then $U=V \iff \dim V=\dim U$. (8.3.4)



## Basis

### Set of vectors $K$, is a basis of the space $V$

Make sure **TWO out of three** are fulfilled (T8.3.2)
1. $K$ is indep. lin. 
2. $\text{Sp}(K)=V$  (K spans V)
3. $|K|=\dim{V}$ 


### (8.4.5)

let $B={(v_{1},v_{2},\dots,v_{n})}$ is a basis of the space $V$ ($n$-dim.), on $F$, then $B'={(u_{1},u_{2},\dots,u_{n})}$ is a basis of $V$, iff the transformation matrix from $B$ to $B'$ is invertible.

## Span

#### Set of vectors $K$, spans the space $V$

https://math.stackexchange.com/questions/56201/how-to-tell-if-a-set-of-vectors-spans-a-space

