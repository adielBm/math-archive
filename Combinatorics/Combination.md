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
can also be used for number of **nonnegative** solutions^[for the equation $x_1+x_2=10$, there are also solution $6+4=10$ and $4+6=10$ and these are considered as two solution. for consider them as a single solution use in Partition https://en.wikipedia.org/wiki/Partition_(number_theory)] of equation $t_1+\cdots+t_n=k$. i.e. the number of solutions is: $$\binom{n+k-1}{k}=\binom{n+k-1}{n-1}$$.

#### Restrictions
##### Minimum restrictions
e.g: **positive** solutions ($t_i \ge 1$ for any $i \le n$) for $t_1+\cdots+t_n=k$ need to add $-1\cdot n$ to $k$
$$\binom{k-1}{n-1}$$

e.g for $t_1$.  solutions for $t_1+\cdots+t_n=k$ such that $t_1 \ge p$. 
$$\binom{n+k-p-1}{k-p}$$

##### Maximum restrictions
e.g. for $t_1$: solutions for $t_1+\cdots+t_n=k$ such that $t_1 \le p$. 
$$\binom{n+k-1}{k}-\binom{n+k-(p+1)-1}{k-(p+1)}$$

or by another method: [[Generating function]]

#### number solutions of inequality
number of **nonnegative** solutions of equation $t_1+\cdots+t_n \leq k$. i.e. the number of solutions is: $$\binom{(n+1)+k-1}{(n+1)-1}=\binom{n+k}{n}$$


