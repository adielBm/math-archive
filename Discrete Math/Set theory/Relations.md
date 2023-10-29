For all $a,b$ and $R\ne \emptyset$
- **Reflexive** - $aRa$
- **Irreflexive** - not $aRa$
- **Symmetric** - $aRb \implies bRA$
- **Antisymmetric** - $aRb \land bRA \implies a=b$
- **Asymmetric** - $aRb \implies$ not $bRa$
- **Connected** - $a\neq{b} \implies aRb \lor bRA$

## Transitive Relations 

> **TRUE** means this property is assigned by definition, or it follows from the definition (for example, Asymmetry follows from transitivity and irreflexivity; irreflexivity follows from asymmetry). Otherwise (empty cell), it indicates that the property is not guaranteed in general; it might or might not hold.


|                                             | Reflexive | Irreflexive | Symmetric | Antisymmetric | Asymmetric | Connected |
| ------------------------------------------- | --------- | ----------- | --------- | ------------- | ---------- | --------- |
| [[#Equivalence relation]]                   | TRUE  |             | TRUE  |               |            |           |
| **Strict partial order**   |           | TRUE    |           | TRUE        | TRUE     |           |
| **Strict total order** |           | TRUE    |           | TRUE        | TRUE     | TRUE  |

- **strict partial order** definitions
	- transitive, irreflexive
	- transitive, asymmetric
- **strict total order** definitions
	- transitive, connected, irreflexive
	- transitive, connected, asymmetric

# Theorems
## Reflexivity

- (q18) - if $R$ reflexive, then $R\subseteq{R^2}$
- (q20a) - if $R\subseteq{S}$ reflexive, then $S$ also reflexive
- (q20b) - if $R$ reflexive, then ${R^2}$ also reflexive
- (q20c) - $R$ reflexive, if and only if, $R^{-1}$ also reflexive 
- (q20d) - if $R,S$ are reflexive, then $R\cap{S},R\cup{S}$ are reflexive
- (q22) - if $R$ is irreflexive, then $S\subseteq{R}$ is also irreflexive

## Symmetry

- (q23) - $R$ is symmetric if and only if $R^{-1} = R$ 
- (q24) - composite of symmetric relations is symmetric
- (q26) - if $R,S$ are symmetric, then $R\cap{S},R\cup{S}$ are symmetric
- (q27) - let $R$ relation, then $R\cap{R}^{-1}$ and $R\cup{R}^{-1}$ are symmetric
- (d2.10) - asymmetric implies antisymmetric
- (q29) - asymmetry implies **irreflexivity**
- (q54a) - **Irreflexivity** and **transitivity** together imply asymmetry
- (q30a) - if $R$ is asymmetric, then $R^{-1}$ is also asymmetric
- (q30b) - if $R$ is antisymmetric, then $R^{-1}$ is also antisymmetric
- (q31a) -  if $R$ is asymmetric, then $S\subseteq{R}$ is also asymmetric.
- (q31b) -  if $R$ is antisymmetric, then $S\subseteq{R}$ is also antisymmetric.
- (q32b) - if $R,S$ are asymmetric, then $R\cap{S}$ is asymmetric
- (q33b) - if $R,S$ are antisymmetric, then $R\cap{S}$ is antisymmetric

## Transitivity

- (theorem 2.12) $R$ is transitive if and only if $R^2\subseteq{R}$
- (q36a) - if $R,S$ are transitive, then $R\cap{S}$ is transitive

# Converse relation
converse relation $R^{-1}$, of a binary relation $R$, is the relation that occurs when the order of the elements is switched in the relation

- If a **relation** is reflexive, irreflexive, symmetric, antisymmetric, asymmetric, transitive, connected, trichotomous, a partial order, total order, strict weak order, total preorder (weak order), or an equivalence relation, **its converse is too**.
- Let $R$ relation from $A$ to $B$, and $S$ relation from $B$ to $C$, then $(RS)^{-1}=S^{-1}R^{-1}$. ^[q69]


# Complementary relation
A binary relation $R$ defined as a subset of a product of sets $A\times B$. The complementary relation $\overline{R}$ is the set complement of $R$ in $A\times{B}$. The complement of relation $R$ can be written $\overline{R}=(A\times{B})\setminus{R}$.


# Composition of relations
let $R_1$ relation from $A$ to $B$, and $R_2$ relation from $B$ to $C$, then 
$$aR_1R_2c\Leftrightarrow\exists{b}\in{B}(aR_1b\land bR_2c)$$
## Properties
- Composition of relations is associative: $R(ST)=(RS)T$

## Relation squared
Let $R$ relation on $A$. then
$$aR^2b\Leftrightarrow\exists{x}\in{A}(aRx\land xRb)$$
# Equivalence relation

- An **equivalence relation** is a binary relation $R$ on $A$ that is **reflexive**, **symmetric** and **transitive**
- The **quotient set** $A/R$ is the set of equivalence classes.
- The **equivalence class** of $a\in{A}$ under equivalence relation $R$ is the set $[a]=\{x \in A : x R a\}$ ^[20476 notation: $\overline{a}$]
- The [[Bell numbers|Bell number]] $B_{n}$ counts **the number of different ways to partition a set** that has exactly $n$ elements, or equivalently, **the number of equivalence relations** on it.

#### Theorems 
- (q43) if $E_1, E_2$ are equivalence relations on a set $A$, then $E_1\cap{E_2}$ is also equivalence relation on $A$.

## Partition of a set
 - A **partition of a set** (quotient set) is a grouping of its elements into non-empty subsets that called **cells** (equivalence classes), in such a way that every element is included in exactly one subset.
 - Every equivalence relation on a set defines a partition of this set, and every partition defines an equivalence relation. (theorem 2.16)
 - A partition $P_1$ is called a **refinement** ^[עידון] of the partition $P_2$ if every set in $P_1$ is a subset of one of the sets in $P_2$.