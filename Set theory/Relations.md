a### Properties

For all $a,b$ and $S\ne \emptyset :$
- **Reflexive** - $aRa$
- **Irreflexive** - not $aRa$
- **Symmetric** - $aRb \implies bRA$
- **Antisymmetric** ^[20476: אנטי סימטרי במובן הרחב] - $aRb \land bRA \implies a=b$
- **Asymmetric** ^[20476: אנטי סימטרי] - $aRb \implies$ not $bRa$
- **Connected** - $a=b \implies aRb \lor bRA$

### Theorems
- question 29 - Asymmetric Relation is Antireflexive
- Asymmetric Relation is Antisymmetric
- question 23 - $R$ is symmetric if and only if it equals its inverse: $R^{-1} = R$ 
- question 24 - Composite of Symmetric Relations is Symmetric

### Transitive realtions 

|                                             |  Reflexive |  Irreflexive |  Symmetric |  Antisymmetric |  Asymmetric |  Connected |
| ------------------------------------------- | ---------- | ------------ | ---------- | -------------- | ----------- | ---------- |
|  Equivalence relation                       | TRUE       |              | TRUE       |                |             |            |
|  Preorder (Quasiorder)                      | TRUE       |              |            |                |             |            |
|  Partial order, (סדר חלקי 80181, חלש)       | TRUE       |              |            | TRUE           |             |            |
|  Total preorder                             | TRUE       |              |            |                |             | TRUE       |
|  Total order, linear order, (מלא, ליניארי)  | TRUE       |              |            | TRUE           |             | TRUE       |
|  Prewellordering                            | TRUE       |              |            |                |             | TRUE       |
|  Well-quasi-ordering                        | TRUE       |              |            |                |             |            |
|  Well-ordering                              | TRUE       |              |            | TRUE           |             | TRUE       |
|  Lattice                                    | TRUE       |              |            | TRUE           |             |            |
|  Join-semilattice                           | TRUE       |              |            | TRUE           |             |            |
|  Meet-semilattice                           | TRUE       |              |            | TRUE           |             |            |
|  Strict partial order,(סדר חלקי 20476, חזק) |            | TRUE         |            |                | TRUE        |            |
|  Strict weak order                          |            | TRUE         |            |                | TRUE        |            |
|  Strict total order                         |            | TRUE         |            |                | TRUE        | TRUE       |

### Converse relation
converse relation $R^{-1}$, of a binary relation $R$, is the relation that occurs when the order of the elements is switched in the relation

- If a **relation** is reflexive, irreflexive, symmetric, antisymmetric, asymmetric, transitive, connected, trichotomous, a partial order, total order, strict weak order, total preorder (weak order), or an equivalence relation, **its converse is too**.

### Complementary relation
A binary relation $R$ defined as a subset of a product of sets $A\times B$. The complementary relation $\overline{R}$ is the set complement of $R$ in $A\times{B}$. The complement of relation $R$ can be written $\overline{R}=(A\times{B})\setminus{R}$.


### Composition of relations
let $R_1$ relation from $A$ to $B$, and $R_2$ relation from $B$ to $C$, then 
$$aR_1R_2c\Leftrightarrow\exists{b}\in{B}(aR_1b\land bR_2c)$$
##### Relation squared
Let $R$ relation on $A$. then
$$aR^2b\Leftrightarrow\exists{x}\in{A}(aRx\land xRb)$$
