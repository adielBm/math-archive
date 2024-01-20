# Unit 1

## (1.43) Bernoulli's Inequality 
 $$x>-1\implies\forall n \in \mathbb{N},({1 + x})^n \ge 1 + n x$$

| Proof by Induction |  |
| ---- | ---- |
| base case |  |
| $n=1\implies 1+x\geq 1+x$ |  |
| induction step |  |
| $({1 + x})^n \ge 1 + n x$ | induction hypothesis |
| $(1+x )({1 + x})^n \ge(1+x )(1 + n x)$ | multiplying by $(1+x)\geq 0$ (because $x>-1$) |
| $({1 + x})^{n+1} \ge1+x+nx+nx^2$ |  |
| $({1 + x})^{n+1} \ge 1+(n+1)x+nx^2$ |  |
| $(1+x)^{n+1}\geq 1+(n+1)x$ | because $nx^2\geq 0$ |
## (1.47) Existence minimum and maximum of set 

- Let $A = \{x_1, \ldots,x_n\}$ be a **nonempty** finite set of size $n > 0$. Then there exist some $m,M \in A$ such that for all $x \in S$, we have that $m \leq x \leq M$

| Proof by Induction (for maximum) |  |
| ---- | ---- |
| **Base Case** |  |
| For $n=1$, let $A=\{x_1\}$ |  |
| $M=x_1$ | Trivially, $M=x_1$ holds |
| **Induction Step** |  |
| $\exists M:\forall x \in A,\,x\leq M$ | Inductive hypothesis |
| if $x_{n+1}>\max\{ x_{1},\dots,x_{n} \}$ then $M:=x_{n+1}$<br>if $x_{n+1}\leq\max\{ x_{1},\dots,x_{n} \}$ then $M:=\max\{ x_{1},\dots,x_{n} \}$ |  |
# Unit 2
## (2.12) Limit Uniqueness

Let $(a_n)$ be a convergent sequence
$$( \lim_{ n \to \infty } a_{n}=L \land{\lim_{ n \to \infty } a_{n}=M})\implies{L=M}$$

#todo check it!!

| Proof by Contradiction |  |
| ---- | ---- |
| $L\neq M$ | Assume by contradiction |
| $\displaystyle\varepsilon=\frac{\vert L-M\vert}{3}>0$ | because $L\neq M$ |
| $\exists N_{1}:\forall n>N_{1},\vert{a_{n}-L}\vert<\varepsilon$ | because $\displaystyle{\lim_{ n \to \infty } a_{n}=L}$ |
| $\exists N_{2}:\forall n>N_{2},\vert{a_{n}-M}\vert<\varepsilon$ | because $\displaystyle{\lim_{ n \to \infty } a_{n}=M}$ |
| $n:=\max\{ N_{1}, N_{2} \}+1$ |  |
| $n>N_{1},n>N_{2}$ |  |
| $\vert{a_{n}-L}\vert<\varepsilon,\vert{a_{n}-M}\vert<\varepsilon$ |  |
| $\vert{L-M}\vert \leq \vert{a_{n}-L}\vert + \vert{a_{n}-M}\vert$ | Triangle inequality |
| $\vert{L-M}\vert < \varepsilon + \varepsilon$ |  |
| $\vert{L-M}\vert < \frac{\vert L-M\vert}{3} + \frac{\vert L-M\vert}{3}$ | Substituting $\varepsilon$ |
| $\vert{L-M}\vert < \frac{2\vert L-M\vert}{3}$ | Combining like terms |
| $3\vert{L-M}\vert < 2\vert L-M\vert$ | Multiplying both sides by 3 |
| $3<2$ | Dividing by $\vert L-M\vert$ both sides |
| **Contradiction!** |  |
|  |  |

## (2.16) Convergent sequence is Bounded

| Proof by #todo  |  |
| ---- | ---- |
| a |  |


## (2.22)

## (2.26)



## (2.32)


## (2.43e)


## (2.47)



# Unit 3

## (3.10)

