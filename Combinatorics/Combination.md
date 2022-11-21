## k-combination
*binomial coefficient*
$$C(n,k)=\binom{n}{k}=\frac{n!}{k!(n-k)!}$$

## combination with repetitions (Stars and Bars)
**<u>There are those who exchange n with k!!!!</u>

*k-combination with repetitions*, or *k-multicombination*, or *multisubst* or *צירופים עם חזרות*

**Stars and Bars** also called *sticks and stones*, *balls and bars*, and *dots and dividers*.

how many ways there are to put **n indistinguishable balls into k distinguishable Bars**.

$$\left(\!\!{k\choose n}\!\!\right)=\binom{n+k-1}{k-1}=\binom{n+k-1}{n}$$
k = Bars (תאים) distinguishable (שונים)
n = Balls (כדורים) indistinguishable (זהים)

can also be used for number of **nonnegative** solutions of equation: $x_1+\cdots+x_k=n$.

#### Restrictions
**positive** solutions ($x_i > 0$) for $x_1+\cdots+x_k=n$ is: 
$$\binom{n-1}{k-1}$$
note: if x_i >= r, so stars = n - r  
e.g. if x_1 >= 2, and x_2 >= 1, so stars = 10 - 2 - 1 = 7.
