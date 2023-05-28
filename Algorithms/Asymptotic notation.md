
| Name                 | examples            | Running Time           |
| -------------------- | ------------------- | ---------------------- |
| constant time        | $c$                 | $O(1)$                 |
| log-logarithmic      |                     | $O(\log{\log n})$      |
| logarithmic time     | $\log n, \log(n^2)$ | $O(\log{n})$           |
| polylogarithmic time | $(\log n)^2$        | $O((\log n)^c)$, $c>1$ |
| fractional power     |                     | $O(n^c)$, $0<c<1$      |
| linear time          |                     | $O({n})$               |
| linearithmic time    |                     |                        |
| quasilinear time     |                     |                        |
| quadratic time       |                     | $O({n^2})$             |
| cubic time           |                     | $O({n^3})$             |
| exponential time     |                     |     $O(c^n), c>1$                   |


- Theorem 3.1 - $f(x)=\Theta({g(n)})\iff{{f(n)=O(g(n))}\land{f(n)=\Omega{(g(n))}}}$



___
draft:
- $O(g(n))=\set{f(n):0\leq{f(n)}\leq{cg(n)},\forall{n\geq{n_0}}}$
- $f(n)=O(g(n))\implies{g(n)=\Omega{(f(n))}}$
