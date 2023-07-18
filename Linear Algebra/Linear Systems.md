## Solving Linear Systems 

- Gaussian elimination (REF)
- Gauss–Jordan elimination (RREF)

## Consistency 

- (8.6.2) **Rouché–Capelli theorem** - $A\mathbf{x}=\mathbf{b}$ is **consistent**, if and only if,  $\rho([A|\mathbf{b}])=\rho(A)$


# Square System



- $A$ an invertible, if and only if, for each $\textbf{b}$, the system of equations $A\textbf{x}=\textbf{b}$ has exactly one solution, namely, $\textbf{x}=A^{−1}\textbf{b}$. 
	- (4.6.1) Cramer's rule: in that case, $\mathbf{x}=(x_{1},\dots,x_{n})$, $x_i = \frac{\det(A_i)}{\det(A)}$, $i = 1, \ldots, n$, where $A_{i}$ is the matrix formed by replacing the $i$-th column of $A$ by the column vector $\mathbf{b}$.

