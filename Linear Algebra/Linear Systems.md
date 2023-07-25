$\large A$ is $m\times n$ matrix 


The following statements are **equivalent**:
- For each $\mathbf{b}\in\mathbb{R}^m$, the equation $A\mathbf{x}=\mathbf{b}$ has a solution
- Each $\mathbf{b}\in\mathbb{R}^m$ is a linear combination of the colmuns of $A$
- The colmuns of $A$ span $\mathbb{R}^m$
- $A$ has a pivot position in every row

## Consistency 

The following statements are **equivalent**:
- $A\mathbf{x}=\mathbf{b}$ is **consistent**
- (8.6.2) **Rouché–Capelli theorem** $\rho([A|\mathbf{b}])=\rho(A)$
- $\text{REF}[A|\mathbf{b}]$ has no row $\left[\begin{array}& 0 & \cdots & 0 & b \end{array}\right]$ with $b$ nonzero 
- $\mathbf{b}$ is a linear combination of the colmuns of $A$

**Properties of consistent system:**
- **number of soltions:**
	- if there are no free variables, there is a unique solution
	- if there is at least one free variable, there are infinitely many solutions


## Homogeneous system
$$\large A\mathbf{x}=\mathbf{0}$$
- homogeneous system is consistent
- $A$ has a nontrivial solution if and only if it has at least one free variable.

# Square System

- $A$ an invertible, if and only if, for each $\textbf{b}$, the system of equations $A\textbf{x}=\textbf{b}$ has exactly one solution, namely, $\textbf{x}=A^{−1}\textbf{b}$. 
	- (4.6.1) Cramer's rule: in that case, $\mathbf{x}=(x_{1},\dots,x_{n})$, $x_i = \frac{\det(A_i)}{\det(A)}$, $i = 1, \ldots, n$, where $A_{i}$ is the matrix formed by replacing the $i$-th column of $A$ by the column vector $\mathbf{b}$.

