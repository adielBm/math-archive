# Existence of an Unique Solution of an Equation given by two differentiable functions

- Given functions $g_1(x), g_2(x)$ that are differentiable on $\mathbb{R}$. Prove that there is only one solution of the equation $g_1(x)=g_2(x)$
	- define $f(x)=g_2(x)-g_1(x)$ i.e. we need to prove these's only one root of $f$
	- $f$ is differentiable (and continuous) on $\mathbb{R}$
	- we need to find $[a,b]$ such that $f(a)<0<f(b)$ (or $f(b)<0<f(a)$)
	- by IVT $\exists c \in[a,b]:f(c)=0$, so $c$ is a root of $f$
	- showing that the root is **unique** by showing that $f$ is (strictly) monotonic by the derivative $f'$. (if for example $f'(x)\neq 0$ then $f$ is monotonic by 8.18; otherwise use in q8.29 or ) 
	- if so $f$ is (strictly) monotonic therefore is one-to-one therefore $c$ is unique root




