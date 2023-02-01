
# Subgraphs

- $G'=(V',E')$ is **subgraph** ^[תת-גרף] of $G$, if $V'\subseteq{V}$ and $E'\subseteq{E}$, and every edge in $E'$ connects two nodes in $V'$
- $G'=(V',E')$ is **spanning subgraph** ^[תת-גרף פורש] of $G$, if is subgraph of $G$, and $V'=V$
- $G'=(V',E')$ is **induced subgraph** ^[תת-גרף מושרה] of $G$ by $V'\subseteq{V}$, such that $vu\in{E} \land {v,u {\in{V'} \iff vu\in{E'}}}$  

# Neighbour

- An **adjacent vertex** ^[צומת שכנה] of a vertex $v$ in a graph is a vertex that is connected to $v$ by an edge. 
- The **neighbourhood of a vertex $v$** ^[קבוצת השכנים של צומת]. $$\Gamma(v) = \set{u \in V \mid (v,u) \in E}$$
- The **neighbourhood of set** ^[קבוצת השכנים של קבוצת צמתים] $A\subseteq{V}$ is the union of the neighbourhoods of the vertices of $A$. $$\Gamma(A)=\bigcup_{v\in{A}}\Gamma(v)$$






