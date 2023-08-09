## Linearity

- Definitions of linearity of transformation. The following statements are **equivalent**:
	- $T$ is **linear** transformation
	- $T$ is additive and homogeneous (9.1.1)
		1. **Additivity:** $T(v_{1}+v_{2})=T(v_{1})+T(v_{2})$
		2. **Homogeneity:** $\alpha T(v)=T(\alpha{v})$
	- $T(\lambda_{1}v_{1}+\lambda_{2}v_{2})=\lambda_{1}T(v_{1})+\lambda_{2}T(v_{2})$ (9.1.3, equivalent to d9.1.1) 
	- There exists $A$ such that $Tv=Av$ for each $v\in{V}$

**Theorems:**
- (9.1.2a) if $T(0_{V})\neq0_{W}$, then $T$ is not linear

**Properties:**
- $T(v)=T(u)\iff T(v-u)=0$

___
$$\large T:V\to W$$
- $A_{m\times n}=[T]^B_{C}$
- $Tv=Av$
- $\dim{V}=n,  \quad\dim{W}=m$
- $B=(v_{1},\dots,v_{n})$ and $C=(w_{1},\dots,w_{m})$ are bases of $V$ and $W$. (respectively) 

## Image

- Definition:
	- $\operatorname{Im}(T) = \{\ T(v) \mid v \in V\,\}$


- (9.3.6) let $T:V\to W$, and $\text{Sp}\{ v_{1},\dots ,v_{n} \}=V$, then, $\text{Im}{T}=\text{Sp}{(\{ T(v_{1}),\dots,T(v_{n}) \})}$
- (9.3.7) let $A_{m \times n}$ matrix on field $F$, and $T:F^n\to F^m$, where $T(v)=Av$, then, $\text{Im}(T)=\text{Col}{(A)}$ (the column space of $A$)
- (9.6.2) if $T:V\to W$ is isomorphism, then $\text{Im}{T}=W$
- $\text{Im}T$ is subspace of $W$

>q9.3.2c, q9.3.3, q9.4.2

- (9.5.6) if $T$ is injective, and $K\subseteq{V}$ independent linearly set, then $T(K)\subseteq{W}$ is also independent linearly set.

## Kernel 

- Definition: $\ker(T) = \{ v \in V : T(v) = 0_W\}$
- (9.3.5) $\ker T$ is subspace of $V$
- (9.5.2) $T$ is injective, if and only if, $\ker{T}=\{ 0 \}$

>see 9.6.2 

## Transformation matrix

(d10.1.1)  Matrix Representations of Linear Transformation
$$[T]_{C}^{B}=\left[\begin{array}{ccc} | & & | \\ [T({v_{1}})]_{C} & \cdots & [T( {v_{n}})]_{C} \\ | & & | \end{array} \right]_{m\times n}$$


> [!example] Compute $T(v)$ Indirectly 
> 1. Compute the coordinate vector $[v]_{B}$
> 2. Compute $[T(v)]_{C}=[T]_{C}^{B}[v]_{B}$
> 3. Reconstruct $T(v)$ from its coordinate vector $[T(v)]_{C}$

## Equality

- (9.4.1) $T,S:V\to W$, and $B=\{ v_{1},\dots,v_{n} \}$ spans $V$. then $T=S \iff \forall{v\in B}:{T(v)=S(v)}$ 

## Surjective (Onto)

The following statements are **equivalent**:
- $T:V\to W$ is surjective
- $A$ columns spans $W$ 
- $\dim V =\dim \text{im} T$
- (T is right-cancellable) $RT=ST\implies R=S$ 
- (T is right-invertible) There exists $S:W\to V$ such that $TS=I$ 


Theorems: 
- if $\dim{V}<\dim{W}$ then $T$ cannot be onto 

## Injective (One-to-One)

Definition: The following statements are **equivalent**:
- $T:V\to W$ is injective
- (9.5.2) $\text{ker}(T)=\set{0}$
- $\dim(\ker{T})=0$
- $T(u)=T(v)\implies u=v$
- The colmuns of $A$ are linearly independent
- (T is left-cancellable) $TR=TS\implies R=S$ 
- (T is left-invertible) There exists $S:W\to V$ such that $ST=I$ 

Theorems: 
- if $\dim{W}<\dim{V}$ then $T$ cannot be one-to-one 
# dimV=dimW

## Theorems

- (9.4.2) Let $B=(v_1,\dots,v_n)$ be a basis of $V$ and $(w_1,\dots,w_n)$ an arbitrary list of vectors in $W$. Then there **exists** a **unique** linear map $T:V\to W$ such that $T(v_{i})=w_{i}$
## Isomorphism

- Definition: The following statements are **equivalent** (9.6.2)
	- $T$ is an **isomorphism** (invertible linear transformation)
	- $T$ is **injective**
	- $T$ is **surjective**
	- $T$ is **bijective**
	- There is $T^{-1}:W\to V$ such that $T^{-1}T=I_{V}$
	- There is $T^{-1}:W\to V$ such that $TT^{-1}=I_{W}$
	- (10.5.1-2) $A=[T]^B_{C}$ is invertible, i.e. $A^{-1}=[T^{-1}]^C_{B}$ exists
	- (9.9.2) the inverse $T^{-1}:W\to V$ exists, such that $T^{-1}T=I_{V}$ and $TT^{-1}=I_{W}$

**Propreties:**
- 

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