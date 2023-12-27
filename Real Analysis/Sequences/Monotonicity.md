
**definitions**
- monotone sequence (either increaseing or decreaseing)
	- monotonically increasing: $a_{n}+1≥a_n$ for all $n\in\mathbb{N}$
		- strictly monotonically increasing: $a_{n}+1>a_n$ for all $n\in\mathbb{N}$
	- monotonically decreasing: $a_{n}+1\leq a_n$ for all $n\in\mathbb{N}$
		- strictly monotonically decreasing: $a_{n}+1<a_n$ for all $n\in\mathbb{N}$

**Theorems**
- Monotone convergence theorem
	- (3.16) if $(a_{n})$ is a **monotone** and **bounded** sequence, then it's convergent
		-  if $(a_{n})$ is **increasing** bounded, then $\lim_{ n \to \infty }(a_{n})=\sup(a_{n})$
		-  if $(a_{n})$ is **decreasing** bounded, then $\lim_{ n \to \infty }(a_{n})=\inf(a_{n})$
	- (3.17) if $(a_{n})$ is a **monotone** and **not-bounded** sequence, then
		-  if $(a_{n})$ is **increasing**, then $\lim_{ n \to \infty }(a_{n})=\infty$
		-  if $(a_{n})$ is **decreasing**, then $\lim_{ n \to \infty }(a_{n})=-\infty$

