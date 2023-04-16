
# Defination 

#### vector addition

| Axioms of *vector addition* |                                                      |                                   |
| --------------------------- | ---------------------------------------------------- | --------------------------------- |
| Closure                     | $\mathbf{a+b}\in{F^{n}}$                             | $\forall{\mathbf{a,b}\in{F^n}}$   |
| Associativity               | $\mathbf{a+(b+c)=(a+b)+c}$                           | $\forall{\mathbf{a,b,c}\in{F^n}}$ |
| Commutativity               | $\mathbf{a+b=b+a}$                                   | $\forall{\mathbf{a,b}\in{F^n}}$   |
| Identity element            | ${\exists}\mathbf{0}\in{F^{n}:{\mathbf{a+0=0+a=a}}}$ | $\forall{\mathbf{a}\in{F^n}}$     |
| Inverse elements            | ${\exists}\mathbf{-a}\in{F^{n}:{\mathbf{a+(-a)=0}}}$ | $\forall{\mathbf{a}\in{F^n}}$     |

#### scalar multiplication

| Axioms of *scalar multiplication*                                 |                                           |                                                    |
| ----------------------------------------------------------------- | ----------------------------------------- | -------------------------------------------------- |
| Closure                                                           | $t\mathbf{a}\in{F^n}$                     | $\forall{\mathbf{a}}\in{F^{n}},\forall{t\in{F}}$   |
| Distributivity of *scalar mul.* with respect to *vector addition* | $t(\mathbf{a+b})=t\mathbf{a}+t\mathbf{b}$ | $\forall{\mathbf{a,b}}\in{F^{n}},\forall{t\in{F}}$ |
| Distributivity of  *scalar mul.* with respect to *field addition* | $(s+t)\mathbf{a}=s\mathbf{a}+t\mathbf{a}$ | $\forall{\mathbf{a}}\in{F^{n}},\forall{s,t\in{F}}$ |
| Compatibility of *scalar mul.* with *field multiplication*        | $(st)\mathbf{a}=s(t\mathbf{a})$           | $\forall{\mathbf{a}}\in{F^{n}},\forall{s,t\in{F}}$ |
| Identity element                                                  | $1\mathbf{a}=\mathbf{a}$                  | $\forall{\mathbf{a}}\in{F^{n}}$                    |


# Geometry of Vector Spaces

#### Line or plane through point, and that is parallel to line or plane

| name                                                                             | parametric form                                        |                                                            |
| -------------------------------------------------------------------------------- | ------------------------------------------------------ | ---------------------------------------------------------- |
| **line** through $\mathbf{b}$ that is parallel to $\mathbf{a}$                   | $\mathbb{R}\mathbf{a+b}$                               | $\mathbf{a,b}$ are non-collinear, and $\mathbf{a\neq{0}}$, |
| **plane** through $\mathbf{c}$ that is parallel to $\mathbf{a}$ and $\mathbf{b}$ | $\mathbb{R}\mathbf{a}+\mathbb{R}\mathbf{b}+\mathbf{c}$ | $\mathbf{a,b}$ are non-collinear                           |

#### Line or plane through 2 or 3 points
| name                                                          | parametric form                                                |                                           |
| ------------------------------------------------------------- | -------------------------------------------------------------- | ----------------------------------------- |
| **line** through $\mathbf{a}$ and $\mathbf{b}$                | $\mathbb{R}(\mathbf{a-b})+\mathbf{b}$                          | $\mathbf{a\neq{b}}$                       |
| **plane** through $\mathbf{a}$, $\mathbf{b}$ and $\mathbf{c}$ | $\mathbb{R}(\mathbf{a-c})+\mathbb{R}(\mathbf{b-c})+\mathbf{c}$ | $\mathbf{a,b,c}$ are non-collinear points |

# Basis

- $S=\mathbf{a}_1,\mathbf{a}_2,\ldots,\mathbf{a}_n$ is called **spanning set/sequence** if any $\mathbf{b}\in{F^n}$ can be written as a *linear combination* $\mathbf{b}=b_1\mathbf{a_1}+b_2\mathbf{a_2}+\cdots+b_n\mathbf{a_n}$. And we say that $S$ spans $F^n$
- $B\subseteq{F^{n}}$ is called **basis**, if is *spanning set*, and *linearly independent*
- The vectors sequence $\mathbf{e}_1,\mathbf{e}_2,\ldots,\mathbf{e}_n$ is **the standart basis** of $F^n$. $$\begin{matrix}\mathbf{e}_1 & = & (1,0,0,\ldots,0) \\ \mathbf{e}_2 & = & (0,1,0,\ldots,0) \\ & \vdots \\ \mathbf{e}_n & = & (0,0,0,\ldots,1)\end{matrix}$$
___

$S$ is set of vectors in vector space $F^n$. each 2 of 3 imply the other.
- $S$ is spanning set
- $S$ is linearly independent
- $|S|=n$ 



