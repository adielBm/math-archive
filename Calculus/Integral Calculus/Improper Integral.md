# Definitions
## Infinite Intervals

| The **improper integral** of $f$                                                                               | $f$ is continuous on |
| -------------------------------------------------------------------------------------------------------------- | -------------------- |
| $\displaystyle\int _{a}^{\infty}f(x) \, dx=\lim_{ t \to\infty }\int _{a}^{t}f(x) \, dx$                        | $[a,\infty)$         |
| $\displaystyle\int _{-\infty}^{b}f(x) \, dx=\lim_{ t \to -\infty }\int _{t}^{b}f(x) \, dx$                     | $(−\infty, b]$       |
| $\displaystyle\int _{-\infty}^{\infty}f(x) \, dx=  \int _{-\infty}^{c}f(x) \, dx+\int _{c}^{\infty}f(x) \, dx$ | $(−\infty, \infty)$  |

If the limits exist, then the improper integrals **converge**; otherwise, they **diverge**.

## Unbounded Integrand

| The **improper integral** of $f$                                                       | $f$ is continuous on |
| -------------------------------------------------------------------------------------- | -------------------- |
| $\displaystyle\int _{a}^{b}f(x) \, dx=\lim_{ t \to a^+ }\int _{t}^{b}f(x) \, dx$       | $(a,b]$              |
| $\displaystyle\int _{a}^{b}f(x) \, dx=\lim_{ t \to b^- }\int _{a}^{t}f(x) \, dx$       | $[a,b)$              |
| $\displaystyle\int _{a}^{b}f(x) \, dx=\int _{a}^{p}f(x) \, dx+\int _{p}^{b}f(x) \, dx$ | $[a,p)\cup(p,b]$     |

- (3.2) given $b>0$, then $\displaystyle\int _{0}^b\frac{dx}{x^\alpha}$ converges if and only if $\alpha<1$
- (3.3) if $f$ is integrable on $[a,b]$ then the improper integral over $(a,b]$ (or $[a,b)$) is equal to the integral over $[a,b]$ 


# Comparison Tests

### Direct Comparison Test

- Let $f$ and $g$ be continuous on $[a,\infty)$ with $0\leq f(x)\leq g(x)$ for all $a\leq x$ then: 
	- if $\int ^{\infty}_{a} g \, dx$ converges then $\int ^{\infty}_{a} f\, dx$ convergent
	- if $\int ^{\infty}_{a} f \, dx$ diverges then $\int ^{\infty}_{a} g\, dx$ diverges

### Limit Comparison Test

- If the positive functions $f$ and $g$ are continuous on $[a, \infty)$, and if $\displaystyle\lim_{ x \to \infty }\frac{f(x)}{g(x)}=L$ where $0<L$ then $\int ^\infty_{a} f \, dx$ and $\int ^\infty_{a} g \, dx$ either both converge or both diverge 


