
# Aritmetic

$U$ and $W$ are subspaces of $V$.

- (q7.6.2) $U\cup W$ is subspace of $V$, if and only if, $U\subseteq W\lor W\subseteq U$ 

- **Sum:** $U + W := \{u+w \mid u\in U , w \in W \}. \tag{4.4.1}$
	- (q7.6.3a) $U+W=W+U$
	- (q7.6.3b) $U_{1}+(U_{2}+U_{3})=(U_{1}+U_{2})+U_{3}$
	- (q7.6.5) $U+W=U\iff W\subseteq U$
	- (q7.6.6) $\text{Sp}(U_{1}\cup\dots \cup U_{k})=U_{1}+\dots+U_{k}$ 
	- (q7.6.7) $U+W=U\cup W$, if and only if, $U\subseteq W\lor W\subseteq U$ 
	- (q7.6.8) let $K,S\subseteq V$ non-empty sets, and $U=\text{Sp}(K)$, $W=\text{Sp}(S)$, then $U+W=\text{Sp}(K\cup S)$
	- **Direct sum**:  $U\oplus{W}=V \iff U+{W}=V$ and $U \cap W=\{ 0 \}$
		- (8.3.7) if $V=U+W$, then $V=U\oplus W \iff \dim V= \dim U+\dim W$ 
	- 

# Equality

- (7.5.12) let $U=\text{Sp}{(S)}$ and $V=\text{Sp}{(T)}$, if the matrix by $S$ as rows, is ***row-equivalent*** to the matrix by $T$ as rows, then $U=V$
- (8.3.4) if $U\subseteq V$ then, $U=V \iff \dim V=\dim U$. 

# Isomorphic Subspaces

- def
- Determine if two subspaces are isomorphic. $V\cong{W}$
	assumption: the spaces are on the same filed $F$  
	- (9.5.7, 9.5.9) $\dim{V}=\dim{W} \iff V\cong{W}$
	- (9.5.8) $\dim{V}=n\implies V\cong{F^n}$

# Dimension 

- (8.3.6) $\dim(U+W)=\dim{U}+\dim{W}-\dim(U \cap W)$
- (8.3.7) if $V=U+W$, then $V=U\oplus W \iff \dim V= \dim U+\dim W$ 
- (9.5.9) $V \cong W \iff \text{dim}{V}=\text{dim}{W}$ (on the same field, and finite dim.)
- (9.6.1) **Rank–nullity theorem** $\text{dim}{V}=\text{dim}{(\text{Ker}{T})}+\text{dim}{(\text{Im}{T})}$. ($T:V\to W$ is lin. trans.)
- (d8.5.4) $\rho{(A)}=\dim(\text{row-space(A)})=\dim(\text{column-space(A)})$

# Orthogonality 

- (d12.2.2) $\mathbf{v} \perp U$ if for all vectors $\mathbf{u} \in U$, $\mathbf{v} \cdot \mathbf{u} = 0$
- (12.2.3) let $K$ spans $U$, then $\mathbf{v} \perp U$, if and only if, $\mathbf{v} \perp K$

## Orthogonal Complement

- (d12.2.4) The **Orthogonal Complement** -  $U^{\perp}=\set{\mathbf{v}\in \mathbb{R}^n  \mid \mathbf{v} \cdot \mathbf{u} = 0, \forall{\mathbf{u} \in U }}$
	- (q12.2.7) ${U^{\perp}}\cap{U}=\{ \mathbf{0} \}$
- (12.3.1) $\text{row-space}(A)\perp\text{null}(A)$
	- $\text{column-space}(A)\perp\text{null}(A^t)$
- (12.3.2) The **Orthogonal Decomposition** of the Euclidean space of dimension $n$. 
	- (12.3.2a) ${U^{\perp}}\oplus{U}=\mathbb{R}^n$
	- (12.3.2a) $\dim U^{\perp}+\dim U=n$
	- (12.3.2b) $(U^\perp)^{\perp}=U$

## Orthogonal Projection

- Definition: the **orthogonal projection** of $\mathbf{a}$ onto $\mathbf{u}$ is $\frac{\mathbf{a}\cdot \mathbf{u}}{\mathbf{u}\cdot \mathbf{u}}\mathbf{u}$.
- Definition: the **orthogonal projection** of $\mathbf{a}$ onto $U\subseteq{\mathbb{R}^n}$ is the vector $$\textbf{u}=\sum^{k}_{i=1}{\frac{\mathbf{a}\cdot \mathbf{u}_{i}}{\| \textbf{u}_{i} \|^2}\textbf{u}_{i}}=\text{proj}_{U}\mathbf{a}$$
	- (where $(\mathbf{u}_{1},\dots,\mathbf{u}_{k})$ is **orthogonal** basis of $U$, and $0\neq\mathbf{a}\in{\mathbb{R}^n}$, and $\mathbf{a}=\mathbf{u}+\mathbf{v}$ where $\mathbf{u}\in{U}$ and $\mathbf{v}\in{U}^{\perp}$) (after12.3.2, 12.4.6)
	- $\mathbf{a}=\mathbf{u}+\mathbf{v}$ is the uniqe form of $\mathbf{a}$ as vector in $U$ and vector in $U^{\perp}$
	- The orthogonal projection of $\mathbf{a}$ onto $U$ is the closest vector to $\mathbf{a}$ in $U$
	- if $(\mathbf{u}_{1},\dots,\mathbf{u}_{k})$ is **orthonormal** basis of $U$, then $\textbf{u}=\sum^{k}_{i=1}{{(\mathbf{a}\cdot \mathbf{u}_{i})}\textbf{u}_{i}}=\text{proj}_{U}\mathbf{a}$
- Projection Theorem - if $\mathbf{v}$ and $\mathbf{u}$ are vectors in $\mathbb{R}^n$, and $\mathbf{u}\neq \mathbf{0}$, then $\mathbf{v}$ can be expressed in excatly one way in the form $\mathbf{v}=t\mathbf{u}+\mathbf{w}$, where $t$ is a scalar, and $\mathbf{w}\perp\mathbf{u}$.

- (12.5.1) $\{ \mathbf{u}_{1},\dots,\mathbf{u}_{k} \}$ is orthogonal set in $\mathbb{R}^n$. and $P(\mathbf{a})$ is the orthogonal projaction of some vector $\mathbf{a}\in \mathbb{R}^n$ onto $\text{Sp}(\{ \mathbf{u}_{1},\dots,\mathbf{u}_{k} \})$, and $\mathbf{v}=\mathbf{a}-P(\mathbf{a})$, then:
	1.  $\mathbf{v}\perp{\{ \mathbf{u}_{1},\dots,\mathbf{u}_{k} \}}$, and $\mathbf{v}\perp{\text{Sp}(\{ \mathbf{u}_{1},\dots,\mathbf{u}_{k} \})}$
	2. $\mathbf{v}=\mathbf{0}\iff \mathbf{a}\in{\text{Sp}(\{ \mathbf{u}_{1},\dots,\mathbf{u}_{k} \})}$


> [!example] Methods
> - given subspace $U$, find the orthogonal projection of $\mathbf{a}$ on $U^{\perp}$. (e2023a.85.q1b)
> 	- find basis for $U$
> 	- find basis for $U^{\perp}$
> 	- normalize this $U^{\perp}$ basis into $(\mathbf{u}_{1},\dots,\mathbf{u}_{k})$
> 	- then $\textbf{u}=\sum^{k}_{i=1}{{(\mathbf{a}\cdot \mathbf{u}_{i})}\textbf{u}_{i}}=\text{proj}_{U^{\perp}}\mathbf{a}$

