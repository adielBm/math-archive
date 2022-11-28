the generating function of the sequance  $a_{0} ,a_{1} ,a_{2} ,\dotsc ,a_{n} ,\dotsc$  is:
$$f( x) =\sum _{n=0}^{\infty } a_{n} x^{n} =a_{0} +a_{1} x+a_{2} x^{2} +\ldots +a_{n} x^{n}$$

## Usage for number of solutions

Generating function can also be used for **number of nonnegative solutions** of equation: $t_1+\cdots+t_n=k$. 
The coefficient of $x^k$ in the following generating function is the number of solutions.
$$f(x)=(1+x+x^2+\ldots+x^k)^n$$
	Remark: coefficient of $x^k$ is $\binom{n-k-1}{n-1}$. see also [[Combination#combination with repetitions (Stars and Bars)]] .

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

