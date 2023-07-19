$$\large{K=\set{{v}_1,\dots,{v}_m}\subseteq V}, \quad \dim{V}=n$$

# Linear independence

Whether $K$ is **linearly independent**?

- **Definition**: $K$ is said to be **linearly independent**, if: $$\lambda_1{v}_1 + \lambda_2{v}_2 + \cdots + \lambda_m{v}_m = {0}\implies{\lambda_{1},\dots,{\lambda_{m}}}=0$$ 
- In other words, if the linear system $Ax=[v_{1},\dots, v_{m}][\lambda_{1},\dots,{\lambda_{m}}]=0$ has only the trivial solution. ($A$ is vectors as comluns)


- ($A$ is $K$'s vectors as **rows**) $\text{rank}({A})=m\leq n\iff K\text{ is linearly {\bf independent}}$.
- if $m=n$, then, $K\text{ is linearly {\bf independent}}\iff A \text{ is {\bf invertible} matrix}$. ($A$ is vectors as comluns/rows)
- $0\in{K}\implies K\text{ is linearly {\bf dependent}}$
- $m>n\implies K\text{ is linearly {\bf dependent}}$

- if $V$ is not the $F^n$ space, (for e.g. *matrices space* or *polynomial space*), then replace the **vecotrs** in the **coordinate vectors**. (q8.2.5, q8.4.1a, q8.4.2a)
- $K$ is linearly independent, if and only if, there is a pivot in every column of the **REF** form of $A$. #todo 

# Span

Whether a set of vectors $K$, spans $V$
- $K\text{ spans }V \iff \text{rank}(\text{REF}(A))=\dim{V}$.   ($A$ is $K$'s vectors as rows)
- $K\text{ spans }V \iff A\mathbf{x}=\mathbf{b}\text{ is consistent}$.   ($A$ is $K$'s vectors as colmuns)
- $B\subseteq{\text{Sp}{(K)}}\implies{K\text{ spans }V}$. (where $\text{Sp}({B})=V$)
- $|{K}|<n\implies K\text{ is {\bf not} span }V$

**Theorems:**
- $\text{Sp}{(K)}=\text{Sp}{(T)}\iff{K\subseteq\text{Sp}{(T)}\land{T\subseteq\text{Sp}{(K)}}}$
- $K\subseteq{\text{Sp}{(T)}}\implies{\text{Sp}{(K)}\subseteq\text{Sp}{(T)}}$
- $K \subseteq{T}\implies{\text{Sp}{(K)}\subseteq\text{Sp}{(T)}}$

# Basis

### finding a basis

#### basis of the **solutions sub-space of** $A\textbf{x}=\textbf{0}$ (*Homogeneous System*) 

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

-  the basis of **the column space** of a matrix $B$, is the basis of **the row space** of a matrix $B^t$,

### basis of the sub-space 

finding basis for $U=\text{Sp}({\set{v_{1},v_{2},\dots,v_{k}   }})\subseteq {F}^n$

reducing a span set to a basis by removing a vectors 
(q8.5.2b)

- set the ${\set{v_{1},v_{2},\dots,v_{k}   }}$ as row vector of matrix, and then follow [[#basis of the row space of a matrix $B$]] 

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

### Extending a linearly independent set to a basis by adding vectors

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

# Orthogonality  

- (d12.2.1) orthogonality of two vectors - $\textbf{a}$ and $\textbf{b}$ are called orthogonal if $\textbf{a}\cdot\textbf{b}=0$ (This relationship is denoted $\textbf{a}\perp\textbf{b}$)
- (q12.2.3) Generalized Theorem of Pythagoras - if $\textbf{a}\perp\textbf{b}$, then  $\| \textbf{a} + \textbf{b} \|^2 = \| \textbf{a} \|^2 +{\| \textbf{b} \|}^2$
- (d12.2.2) $\mathbf{v} \perp U$ if for all vectors $\mathbf{u} \in U$, $\mathbf{v} \cdot \mathbf{u} = 0$
