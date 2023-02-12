**derangement** is a permutation of the elements of a set, such that no element appears in its original position. In other words, a derangement is a **permutation that has no fixed points**. (*אי סדר מלא, בלבול, תמורה ללא נקודות שבת*)

**The number of derangements** of a set of size $n$ is known as the **subfactorial** of $n$ or the $n$-th derangement number or n-th de Montmort number. Notations for subfactorials in common use include $!n$, $D_n$.
$$!n=D_n=(n-1)(D_{n-2}+D_{n-1})$$
or
$$D_n=n! \sum_{i=0}^{n} \frac{(-1)^i}{i!}=n!(1-\frac{1}{1!}+\frac{1}{2!}-\frac{1}{3!}+\ldots+\frac{(-1)^n}{n!})$$



#### Derivation by inclusion–exclusion principle
$$!n = n! - \left|S_1 \cup \dotsm \cup S_n\right| = n! \sum_{i=0}^n \frac{(-1)^i}{i!}$$
>For $1 \leq k \leq n$ we define $S_k$ to be the set of permutations of $n$ objects that fix the $k$-th object. 

