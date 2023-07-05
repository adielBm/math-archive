## Image

finding the image of a linear transformation $\text{Im}T$

- (9.3.6) let $T:V\to W$, and $\text{Sp}\{ v_{1},\dots ,v_{n} \}=V$, then, $\text{Im}{T}=\text{Sp}{(\{ T(v_{1}),\dots,T(v_{n}) \})}$
- (9.3.7) let $A_{m \times n}$ matrix on field $F$, and $T:F^n\to F^m$, where $T(v)=Av$, then, $\text{Im}(T)=\text{Col}{(A)}$ (the column space of $A$)
- (9.6.2) if $T:V\to W$ is isomorphism, and the $\dim{V}=\dim{W}$, then $\text{Im}{T}=W$ (i.e. $T$ is onto)

>q9.3.2c, q9.3.3, q9.4.2

>for Im of indep. subset of V (lin. trans. that is **one-to-one**). see 9.5.6 

## Kernel 

finding the kernel of a linear transformation $\text{Ker}T$

- $\ker(T) = \{ v \in V : T(v) = 0_W\}$

>see 9.6.2 

## linear transformation so that..

- linear transformation $T:V\to W$ s.t. $A=\{ v_{1},\dots ,v_{k} \}$ spans $\text{Ker{(T)}}$
	- find basis to $\text{Ker{(T)}}$
	- take the found basis, and extend it to basis of $F^n$
	- set the Im of the basis 
	- 
	

## Matrix for a Linear Transformation 

$T:V\to W$, and $B=(v_{1},\dots,v_{n})$ and $C=(w_{1},\dots,w_{n})$ are bases of $V$ and $W$. (respectively) 
$$[T]_{C}^{B}=\left[\begin{array}{ccc} | & & | \\ [T({v_{1}})]_{C} & \cdots & [T( {v_{n}})]_{C} \\ | & & | \end{array} \right]_{m\times n}$$

## Compute $T(v)$ Indirectly 

1. Compute the coordinate vector $[v]_{B}$
2. Compute $[T(v)]_{C}=[T]_{C}^{B}[v]_{B}$
3. Reconstruct $T(v)$ from its coordinate vector $[T(v)]_{C}$


## whether a transformation is a linear transformation

given $T:V\to W$
- firstly, check if $T(0_{V})=0_{W}$. 
	- if not, then it's not linearly (9.1.2a). 
	- else, check by d9.1.1, or equivalently by 9.1.3
		- (9.1.3)  $T(\lambda_{1}v_{1}+\lambda_{2}v_{2})=\lambda_{1}T(v_{1})+\lambda_{2}T(v_{2})$

>q9.4.1

## equivalence

whether two linear transformations are equal 

> 9.4.1

## isomorphism

- Definition: linear transformation $T$ is called an isomorphism if is injective and surjective
- Determine if $T:V\to W$ is an isomorphism.
	- (9.6.2) injective $\iff$ surjective $\iff$ isomorphism. (for $V,W$ with the same dim)
	- (10.5.2) if $[T]^B_{C}$ is invertible, then $T$ is isomorphism

# Linear Operator $T:V \to V$

## eigenvalues 

finding the eigenvalues of a Linear Operator 
1. choose some basis $B$ for $V$
2. compute the eigenvalues of the matrix $[T]_{B}$ ([[Matrices#Finding Eigenvalues and Eigenvectors]])

whether a scalar is an eigenvalue of a Linear Operator 
- (d11.2.1) the scalar $\lambda$ is called an **eigenvalue** of $T$, if there is a non-zero vector $v \in V$, such that: $T(v)=\lambda{v}$. And $v$ is called **eigenvector** of $T$ that related to the eigenvalue $\lambda$. 

## Diagonalizability

- (d11.1.1) $T:V\to V$ is **diagonalizable**, if there is a basis for $V$, such that the matrix of $T$ (by this basis), is diagonal.
- (11.2.5) let $T$ is lin. trans. of dim $n$. if $T$ has $n$ **distinct** eigenvalues, then $T$ is diagonalizable
#todo  https://textbooks.math.gatech.edu/ila/diagonalization.html

## characteristic polynomial

- (d11.4.4) the characteristic polynomial of $T:V\to V$ is the characteristic polynomial of the transformation matrix by some basis
- 2