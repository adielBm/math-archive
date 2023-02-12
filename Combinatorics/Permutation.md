- **_k_-permutations of _n_** (חליפה) - $P(n,k)={_n}P_k=\frac{n!}{(n-k)!}=(n)_{k}$
- **_n_-permutations of _n_** (תמורה) - $P(n)=n!$

****

## Permutation with repetition

The number of ways of distribute $k$ distinct objects into $n$ distinct cells (when there is no restriction on the capacities of the boxes, that is, a cell can be empty. ^[If a cell cannot be empty and must contain at least one object, then the number is $n!{\lbrace\textstyle{k\atop n}\rbrace}$ ])
$$n^k$$
___

## Permutations of multisets
^[also called ***multiset permutation*** or ***multinomial theorem*** or ***תמורה עם חזרות*** or **המקדם המולטינומי**]
$$P(n;k_1,k_2,...,k_i)={n \choose k_1, k_2, \ldots, k_i} = \frac{n!}{k_1!k_2! \cdots k_i!}={k_1\choose k_1}{k_1+k_2\choose k_2}\cdots{k_1+k_2+\cdots+k_i\choose k_i}$$


>See also: [[Binomial Coefficient#multinomial coefficient]]

___

##  $k$ distinct objects into $n$ distinct cells
- the order of objects inside the cells is matter
$$k!\binom{n+k-1}{k}=\frac{(n+k-1)!}{(n-1)!} = (n+k-1)^{\underline{k}}$$