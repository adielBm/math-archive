# Sequences of Functions

A sequence of functions is a function whose domain is $\mathbb{N}$ and whose range is a set of functions.

## Convergence

### Pointwise Convergence

- (d6.1) Given a sequence of functions $(f_n)$ that are all defined on an interval $D$, and given a real number $x_0$ in $D$. 
    - (a.) If the sequence of real numbers $(f_n(x_0))$ converges, then we say that the sequence $(f_n)$ **converges** in $x_0$.
    - (b.) If the sequence $(f_n)$ converges in every point of $I\subseteq D$, then we say that the sequence $(f_n)$ **converges (pointwise)** on $I$.
    - (c.) If the sequence $(f_n)$ converges pointwise on $I\subseteq D$, then the function $f$ defined by $\displaystyle f(x) = \lim_{n \to \infty} f_n(x)$ is called the **limit function** of the sequence $(f_n)$ on $I$. In which case, we say that the sequence $(f_n)$ **converges (pointwise) to** $f$ on $I$, and we write $\displaystyle f_n \to f$.
    - In $\varepsilon$-$N$ terms, we say that the sequence $(f_n)$ converges pointwise on $I$ to $f$ if for every $\varepsilon > 0$ and for every $x\in I$, there exists an integer $N$ such that $|f_n(x) - f(x)| < \varepsilon$ for all $n\geq N$. 
        - ($N$ depends on $\varepsilon$ and $x$. So, we can write $N = N(\varepsilon, x)$.)

### Uniform Convergence

- (d6.2) Given a sequence of functions $(f_n)$ defined on an interval $D$. We say that the sequence $(f_n)$ **converges uniformly** to $f$ on $D$ if for every $\varepsilon > 0$, there exists an integer $N$ such that for all $n\geq N$ and for all $x\in D$ we have $|f_n(x) - f(x)| < \varepsilon$. In which case, we say that the sequence $(f_n)$ **converges uniformly** to $f$ on $D$, and we write $\displaystyle f_n \to f$ uniformly on $D$. Also, we say that $f$ is the **uniform limit** of the sequence $(f_n)$ on $D$.
    - ($N$ depends only on $\varepsilon$. So, we can write $N = N(\varepsilon)$.)

- (q6.5) Uniform convergence implies pointwise convergence (but not conversely!).
- (6.3) If $(f_n)$ converges uniformly to $f$ on $I$ if and only if $\displaystyle \lim_{n \to \infty} \sup_{x\in I} |f_n(x) - f(x)| = 0$.


## Series of Functions (6.1.3)

- (d6.2*) #todo
- (6.4) #todo
- (6.4*) #todo
- (6.5) Dini's Theorem - Given a sequence of functions $(f_n)$ defined on an interval $[a,b]$ convergget pointwise to a continuous function $f$ on $[a,b]$. Then, if $(f_n)$ is increasing (i.e. for all $n$ and for all $x\in [a,b]$, we have $f_n(x) \leq f_{n+1}(x)$), then $(f_n)$ converges uniformly to $f$ on $[a,b]$.




- From Spivak:
    - The series of functions $\displaystyle \sum_{n=1}^{\infty} f_n(x)$ converges uniformly (more formally: the sequence $(f_n)$ uniformly summable) to a function $f$ on $I$ if the sequence of partial sums $(S_n)$ converges uniformly to $f$ on $I$, where $\displaystyle S_n(x) = \sum_{k=1}^{n} f_k(x)$.
    - The Weiersstrass M-Test: Let $(f_n)$ be a sequence of functions defined on a set $A$. Suppose that there exists a sequence of positive numbers $(M_n)$ such that for all $n$ and for all $x\in A$, we have $|f_n(x)| \leq M_n$. Suppose moreover that the series $\displaystyle \sum_{n=1}^{\infty} M_n$ converges. Then for each $x\in A$, the series $\displaystyle \sum_{n=1}^{\infty} f_n(x)$ converges (in fact, it converges absolutely), and the series of functions $\displaystyle \sum_{n=1}^{\infty} f_n(x)$ converges uniformly on $A$ to a function $f(x)=\displaystyle \sum_{n=1}^{\infty} f_n(x)$.







- Series of Functions
- Uniform Convergence and Continuity of Limit Function
- Cauchy Test for Uniform Convergence
- Differentiation and Integration Term-by-Term
___


#todo  https://en.wikipedia.org/wiki/Series_expansion