the generating function of the sequance  $a_{0} ,a_{1} ,a_{2} ,\dotsc ,a_{n} ,\dotsc$  is:
$$f( x) =\sum _{n=0}^{\infty } a_{n} x^{n} =a_{0} +a_{1} x+a_{2} x^{2} +\ldots +a_{n} x^{n}$$

## Usage for number of solutions

Generating function can also be used for **number of nonnegative solutions** of equation: $t_1+\cdots+t_n=k$. Then the coefficient of $x^k$ in the following generating function is the number of solutions.
$$f(x)=(1+x+x^2+\ldots)^n=\frac{1}{(1-x)^n}=\sum_{k=0}^{\infty}{\binom{n-k-1}{k}x^k}$$

### Restrictions

#### **Restriction for all Addends**: 
Special case example: a number of solutions of equation: $t_1+\ldots+t_n=k$. **such that** $1 \leq t_i \leq 6$ for any $i \le n$. 
The coefficient of $x^k$ in the following generating function is the number of solutions.
$$f(x)=(x+x^2+\ldots+x^6)^n$$
Example generalization: a number of solutions of equation: $t_1+\ldots+t_n=k$. **such that** $p \leq t_i \leq q$ for any $i \le n$. 
The coefficient of $x^k$ in the following generating function is the number of solutions.
$$f(x)=(x^p+x^{p+1}+\ldots+x^{q-1}+x^q )^n$$

### Equation with Coefficients Greater than 1
Number of solutions of equation $a_1 t_1+a_2 t_2+ \ldots + a_n t_n = k$. ^[question 7.13]
The coefficient of $x^k$ in the following generating function is the number of solutions.
$$f(x)=(1+x^{a_1}+x^{2a_1}+\ldots)(1+x^{a_2}+x^{2a_2}+\ldots)\cdots(1+x^{a_n}+x^{2a_n}+\ldots)$$
## Partition
partition of a positive integer n, also called an integer partition, is a way of writing n as a sum of positive integers. Two sums that differ only in the order of their summands are considered the same partition. 

The partition function $p(n)$ equals the number of possible partitions of a non-negative integer $n$.
The values of this function for $1,2,3,\ldots$ are: (A000041)
$$1, 1, 2, 3, 5, 7, 11, 15, 22, 30, 42, 56,\ldots$$

#### Partition Q (distinct parts)
$Q(n)$, also denoted $q(n)$, gives the number of ways of writing the integer $n$ as a sum of positive integers without regard to order with the constraint that **all integers in a given partition are distinct**. (A000009)
$$1, 1, 2, 2, 3, 4, 5, 6, 8, 10,\ldots$$


# Useful Generating functions

|                      | Generating functions                                               | Sequence                             |
| -------------------- | ------------------------------------------------------------------ | ------------------------------------ |
| Binomial             | $(a+x)^n = \sum_{k=0}^n {n \choose k}a^{n-k}x^k$                   | ${n \choose k}a^{n-k}$               |
| Binomial             | $(1+x)^n = \sum_{k=0}^n {n \choose k}x^k$                          | ${n \choose k}$                      |
| multiset coefficient | $\frac{1}{(1-x)^n}=\sum_{k=0}^\infty {n+k-1 \choose k}x^k=(1+x+x^2+...)^n$         | ${n+k-1 \choose k}$                  |
|                      | $\frac{1}{1-ax}=\sum_{k=0}^\infty a^k x^k = 1+ax+a^2x^2+{\cdots}$  | $a^0,a^1,a^2,a^3,...$                |
|                      |   $\frac{1}{1-x^2}= 1+x^2+x^4{\cdots}$   |  $1,0,1,0,...$                                     |
|                      | $\frac{x}{1-x^2}= x+x^3+x^5{\cdots}$                               | $0,1,0,1,...$                        |
|                      | $\frac{1}{1+x}=\sum_{k=0}^{\infty}(-1)^k x^k=1-x+x^2-x^3+{\cdots}$ | $1,-1,1,-1,...$                      |
| infinite             | $\frac{1}{1-x}=\sum_{k=0}^\infty x^k = 1+x+x^2+{\cdots}$           | $1,1,1,1,...$                        |
| finite               | $\frac{1-x^{n+1}}{1-x}=\sum_{k=0}^n x^k = 1+x+x^2+{\cdots}+x^n$    | $1,1,1,1,...,n$                      |
| ratio                | $\frac{1}{1-x^r}=\sum_{k=0}^\infty x^{kr}=1+x^r+x^{2r}+{\cdots}$   | $c_k=1$ if $r\vert k$ ;  otherwise 0 |


		