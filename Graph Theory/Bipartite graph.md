**bipartite graph** $G=(A \cup B,E)$ is a graph whose vertices can be divided into two disjoint and independent sets $A$ and $B$, that is every edge connects a vertex in $A$ to one in $B$. 

- **Theorem 1.6** - A graph is bipartite if and only if it does not contain an odd cycle.
- **Subgraph of a Bipartite Graph** - Every subgraph H of a bipartite graph G is, itself, bipartite. 
^[question 5].
- **Hall's marriage theorem (4.7)** - The bipartite graph $G=(A \cup B,E)$, Then there exists a  matching that covers $A$ if and only if $|N(X)| \geq |X|$ for all subsets $X$ of $A$.
- **Corollary (4.8) from Hall's marriage theorem** - The bipartite graph $G=(A \cup B,E)$, Then there exists a **perfect matching** if and only if $|N(X)| \geq |X|$ for all subsets $X$ of $A$, and **also** $|A|=|B|$.
- **Kőnig's theorem (4.16)** - In bipartite graphs, the size of minimum vertex cover is equal to the size of the maximum matching. $\beta(G)=\nu(G)$.
- 