
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
