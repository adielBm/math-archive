## Definitions
A tree is undirected graph $G=(V,E)$ that satisfies any of the following equivalent conditions:
- $G$ is connected, acyclic (contain no cycles)
- $G$ is connected, and $|E|=|V|-1$
- $G$ has no simple cycles, and $|E|=|V|-1$

### Leaf
- A leaf of an (unrooted) tree is a vertex degree 1

## Theorems
- Tree with at least 2 vertices has **at least 2 leaves**. (question 2.3)

# Forest

## Definitions
- **forest** is an acyclic graph
- **forest** is an graph in which any two vertices are connected by at most one path

## Properties of Forest
- every of component in forest is tree
- $k$ is number of components (trees) in forest
$$k=|V|-|E| \text{ or } |E|=|V|-k$$

# Cayley's formula

- **Prüfer sequence** of a labeled tree is a unique sequence associated with the tree. The sequence for a tree on $n$ vertices has length $n−2$
- There is **Bijection between Prüfer Sequences and Labeled Trees.** That is, every labeled tree has a unique Prüfer sequence that defines it, and every Prüfer sequence defines just one labeled tree. 
- **Cayley's formula** (2.9) - The number of labeled trees with $n$ vertices is $n^{n−2}$

todo...
התגים שמופיעים בסדרת פרופר הם לא עלים ודרגתם לפי מספר ההופעות.
השאר שאינם בסדרה, הם עלים, כלומר דרגתם 1.
