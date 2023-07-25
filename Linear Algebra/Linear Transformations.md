## Linearly

Whether a transformation $T:V\to W$ is a **linear** transformation?

- (Definition 9.1.1) 
	1. **Additivity:** $T(v_{1}+v_{2})=T(v_{1})+T(v_{2})$
	2. **Homogeneity:** $\alpha T(v)=T(\alpha{v})$
- $T(\lambda_{1}v_{1}+\lambda_{2}v_{2})=\lambda_{1}T(v_{1})+\lambda_{2}T(v_{2})$ (9.1.3, equivalent to d9.1.1) 
- (9.1.2a) if $T(0_{V})\neq0_{W}$, then $T$ is not linearly

>q9.4.1

- $T(v)=T(u)\iff T(v-u)=0$

## Image

finding the image of a linear transformation $\text{Im}T$

- Definition: $\operatorname{Im}(T) = \{\,w \in W: w = T(v), v \in V\,\}$
- (9.3.6) let $T:V\to W$, and $\text{Sp}\{ v_{1},\dots ,v_{n} \}=V$, then, $\text{Im}{T}=\text{Sp}{(\{ T(v_{1}),\dots,T(v_{n}) \})}$
- (9.3.7) let $A_{m \times n}$ matrix on field $F$, and $T:F^n\to F^m$, where $T(v)=Av$, then, $\text{Im}(T)=\text{Col}{(A)}$ (the column space of $A$)
- (9.6.2) if $T:V\to W$ is isomorphism, and the $\dim{V}=\dim{W}$, then $\text{Im}{T}=W$ (i.e. $T$ is onto)
- $\text{Im}T$ is subspace of $W$

>q9.3.2c, q9.3.3, q9.4.2

>for Im of indep. subset of V (lin. trans. that is **one-to-one**). see 9.5.6 

## Kernel 

- Definition: $\ker(T) = \{ v \in V : T(v) = 0_W\}$
- (9.3.5) $\ker T$ is subspace of $V$
- (9.5.2) $T:V\to W$ is injective, if and only if, $\ker{T}=\{ 0 \}$

>see 9.6.2 

## Transformation matrix

Matrix Representations of Linear Transformation

- (d10.1.1) $T:V\to W$, and $B=(v_{1},\dots,v_{n})$ and $C=(w_{1},\dots,w_{n})$ are bases of $V$ and $W$. (respectively) 
$$[T]_{C}^{B}=\left[\begin{array}{ccc} | & & | \\ [T({v_{1}})]_{C} & \cdots & [T( {v_{n}})]_{C} \\ | & & | \end{array} \right]_{m\times n}$$


> [!example] Compute $T(v)$ Indirectly 
> 1. Compute the coordinate vector $[v]_{B}$
> 2. Compute $[T(v)]_{C}=[T]_{C}^{B}[v]_{B}$
> 3. Reconstruct $T(v)$ from its coordinate vector $[T(v)]_{C}$

## Equality

- (9.4.1) $T,S:V\to W$, and $B=\{ v_{1},\dots,v_{n} \}$ spans $V$. then $T=S \iff \forall{v\in B}:{T(v)=S(v)}$ 

# dimV=dimW

## Isomorphism

- Definition: An **isomorphism** is an **invertible linear transformation** (i.e. bijective linear transformation).

- Determine if $T:V\to W$ is an isomorphism?
	- (9.6.2)  if $\dim{V}=\dim{W}$ (finite-dimensional) then, injective $\iff$ surjective $\iff$ isomorphism
	- (10.5.2) if $[T]^B_{C}$ is invertible, then $T$ is isomorphism
	- (9.9.2) if exists $S:W\to V$ such that $ST=I_{V}$ and $TS=I_{W}$, then, $T$ is an isomorphism, $S=T^{-1}$
	- (9.6.2)  if $\dim{V}=\dim{W}$, then the following statements are **equivalent**:
		- $T$ is an isomorphism
		- there is $S:W\to V$ such that $ST=I_{V}$
		- there is $S:W\to V$ such that $TS=I_{W}$

- (9.5.2) $T:V\to W$ is injective, if and only if, $\ker{T}=\{ 0 \}$

## Linear Operator $T:V \to V$

- $T^2=0\implies\mathrm{Im}T\subseteq\mathrm{Ker}T$

### eigenvalues 

finding the eigenvalues of a Linear Operator 
1. choose some basis $B$ for $V$
2. compute the eigenvalues of the matrix $[T]_{B}$ ([[Matrices#Finding Eigenvalues and Eigenvectors]])

whether a scalar is an eigenvalue of a Linear Operator 
- (d11.2.1) the scalar $\lambda$ is called an **eigenvalue** of $T$, if there is a non-zero vector $v \in V$, such that: $T(v)=\lambda{v}$. And $v$ is called **eigenvector** of $T$ that related to the eigenvalue $\lambda$. 

### Diagonalizability

- (d11.1.1) $T:V\to V$ is **diagonalizable**, if there is a basis for $V$, such that the matrix of $T$ (by this basis), is diagonal.
- (11.2.5) let $T$ is lin. trans. of dim $n$. if $T$ has $n$ **distinct** eigenvalues, then $T$ is diagonalizable
#todo  https://textbooks.math.gatech.edu/ila/diagonalization.html

### characteristic polynomial

- (d11.4.4) the characteristic polynomial of $T:V\to V$ is the characteristic polynomial of the transformation matrix by some basis
- 2