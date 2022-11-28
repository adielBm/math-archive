## k-combination (_n_ choose _k_)
*binomial coefficient*
$$C(n,k)=\binom{n}{k}=\binom{n}{n-k}=\frac{n!}{k!(n-k)!}$$

## Combination with Repetitions (Stars and Bars)
combination with repetitions also called *k-combination with repetitions*, or *k-multicombination*, or *multisubst* or *צירופים עם חזרות*. and could be pronounced _n_ multichoose _k_.

**Stars and Bars** also called *sticks and stones*, *balls and bars*, and *dots and dividers*.

how many ways there are to put **k indistinguishable balls into n distinguishable Bars**.

$$D(n,k)=\left(\!\!{n\choose k}\!\!\right)=\binom{n+k-1}{n-1}=\binom{n+k-1}{k}=\frac{(n+k-1)!}{k!\,(n-1)!}$$
n = Bars (תאים) distinguishable (שונים).

k = Balls (כדורים) indistinguishable (זהים).

**<u>There are those who exchange n with k!!!!</u>

### Usage for number of solutions of equation
can also be used for number of **nonnegative** solutions of equation $t_1+\cdots+t_n=k$. i.e. the number of solutions is: $\binom{n+k-1}{k}$.

#### Restrictions
**Minimum restrictions**:
e.g: **positive** solutions ($x_i > 0$) for $x_1+\cdots+x_n=k$ need to add $-1\cdot n$ to $k$
$$\binom{k-1}{n-1}$$
**Maximum restrictions**:
see [[Generating function]]
