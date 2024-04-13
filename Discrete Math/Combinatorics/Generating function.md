#todo read https://enumeration.ca/toolbox/generating-functions/

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

> See [[Partition]]

# Useful Generating functions

|                      | Generating function                                                                   | Sequence $c_0,c_1,c_2,\ldots,c_k,\ldots$ |                                      |
| -------------------- | ------------------------------------------------------------------------------------- | ---------------------------------------- | ------------------------------------ |
| Finite geometric     | $\frac{1-x^{n+1}}{1-x}=\frac{x^{n+1}-1}{x-1}=\sum_{k=0}^n x^k = 1+x+x^2+{\cdots}+x^n$ | $1,1,1,1,...,n$                          |                                      |
| Infinite geometric   | $\frac{1}{1-x}=\sum_{k=0}^\infty x^k = 1+x+x^2+{\cdots}$                              | $1,1,1,1,...$                            |                                      |
| ratio                | $\frac{1}{1-x^r}=\sum_{k=0}^\infty x^{kr}=1+x^r+x^{2r}+{\cdots}$                      |                                          | $c_k=1$ if $r\vert k$ ;  otherwise 0 |
|                      | $\frac{1}{1-ax}=\sum_{k=0}^\infty a^k x^k = 1+ax+a^2x^2+{\cdots}$                     | $a^0,a^1,a^2,a^3,...$                    | $a^k$                                |
|                      | $\frac{1}{1-x^2}=\sum^{\infty}_{k=0}x^{2k}=1+x^2+x^4{\cdots}$                         | $1,0,1,0,...$                            |                                      |
|                      | $\frac{x}{1-x^2}=\sum^{\infty}_{k=0}x^{2k+1}=x+x^3+x^5{\cdots}$                       | $0,1,0,1,...$                            |                                      |
|                      | $\frac{1}{1+x}=\sum_{k=0}^{\infty}(-1)^k x^k=1-x+x^2-x^3+{\cdots}$                    | $1,-1,1,-1,...$                          |                                      |
| exponential function | $e^x=\sum_{k=0}^\infty{x^k \over k!}=1+x+\frac{x^2}{2!}+\frac{x^3}{3!}+\cdots$        |                                          | $\frac{1}{k!}$                       |

## Binomial coefficient

|                         | Generating function                                    |                         |
| ----------------------- | ------------------------------------------------------ | ----------------------- |
| basic                   | $(1+x)^n = \sum_{k=0}^n {n \choose k}x^k$              | ${n \choose k}$         |
| multiplied by $a^{n-k}$ | $(a+x)^n = \sum_{k=0}^n {n \choose k}a^{n-k}x^k$       | ${n \choose k}a^{n-k}$  |
| multiplied by $(-1)^k$  | $(1-x)^n = \sum_{k=0}^{n}{(-1)^k}{n \choose k}x^k$     | ${(-1)^k}{n \choose k}$ |
|                         | $(1+x^m)^n = \sum_{k=0}^n {n \choose k}x^{mk}$         | ${n \choose k}$         |
|                         | $(1-x^m)^n = \sum_{k=0}^n (-1)^{k}{n \choose k}x^{mk}$ | ${n \choose k}$         |

## Multiset coefficient

| | Generating function | |
| -- | -- | -- | -- | 
| basic | $\frac{1}{(1-x)^n}=\sum_{k=0}^\infty {n+k-1 \choose k}x^k=(1+x+x^2+...)^n$ |                      | ${n+k-1 \choose k}$     |
|  multiplied by $(-1)^k$    | $\frac{1}{(1+x)^n}=\sum_{k=0}^\infty (-1)^k{n+k-1 \choose k}x^k=(1-x+x^2-...)^n$ |                      | $(-1)^k{n+k-1 \choose k}$     |
|  $n=2$                    | $\frac{1}{(1-x)^2}=\sum_{k=0}^\infty {(k+1)}x^k=1+2x+3x^2+\ldots$          | $1,2,3,\ldots$                           | $k+1$    |
|  $n=2$, and multiplied by $x$                    | $\frac{x}{(1-x)^2}=\sum_{k=0}^\infty {k}x^k=x+2x^2+3x^3+\ldots$          | $0,1,2,\ldots$                           | $k$    |
| multiplied by $a^k$  | $\frac{1}{(1-ax)^n}=\sum_{k=0}^\infty a^k{n+k-1 \choose k}x^k=(1+ax+a^2x^2+...)^n$ |                      | $a^k{n+k-1 \choose k}$     |


### useful identities of factoring out  

- $(x^3+x^4+\cdots)^n=(x^3)^n(1+x+x^2+\cdots)^n$
- $(x+x^2+x^4+x^5+x^7+\ldots)^n=(x+x^2)^n(1+x^3+x^6+\ldots)^n$
- $(1+x^2+x^3+\cdots)^n=(\frac{1}{1-x}-x)^n=(1-x(1-x))^n{\frac{1}{(1-x)^n}}=(1-x+x^2)^n\frac{1}{(1-x)^n}$
- $(1-x)^3=(1-x)(1+x+x^2)$

