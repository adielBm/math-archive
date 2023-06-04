## Matrices 

### two matrices are row equivalent

#todo 

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

- Option 1: check if $U=\text{Sp}{(S)}$ is equel to $V=\text{Sp}{(T)}$
	- check if the matrix by S as rows, is ***row-equivalent*** to the matrix by T as rows (7.5.12)
- Option 2: if $U\subseteq V$ then $U=V \iff \dim V=\dim U$. (8.3.4)

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

## Linear Transformation

### whether given transformation is linear transformation

given $T:V\to W$
- firstly, check if $T(0_{V})=0_{W}$. 
	- if not, then it's not linearly (9.1.2a). 
	- else, check by d9.1.1, or equivalently by 9.1.3
		- (9.1.3)  $T(\lambda_{1}v_{1}+\lambda_{2}v_{2})=\lambda_{1}T(v_{1})+\lambda_{2}T(v_{2})$

>q9.4.1

### two linear transformations are equel 

- 9.4.1
