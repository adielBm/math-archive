# Definetions 

For all $a,b$ and $R\ne \emptyset$
- **Reflexive** - $aRa$
- **Irreflexive** - not $aRa$
- **Symmetric** - $aRb \implies bRA$
- **Antisymmetric** ^[20476: אנטי סימטרי במובן הרחב] - $aRb \land bRA \implies a=b$
- **Asymmetric** ^[20476: אנטי סימטרי] - $aRb \implies$ not $bRa$
- **Connected** - $a\neq{b} \implies aRb \lor bRA$

## Transitive Relations 

|                                                | Reflexive | Irreflexive | Symmetric | Antisymmetric | Asymmetric | Connected |
| ---------------------------------------------- | --------- | ----------- | --------- | ------------- | ---------- | --------- |
| [[#Equivalence relation]]                      | TRUE      |             | TRUE      |               |            |           |
| **Strict partial order,(סדר חלקי 20476)** |           | TRUE        |           |               | TRUE       |           |
|  **Strict total order, (יחס סדר מלא 20476)**                         |            | TRUE         |            |                | TRUE        | TRUE       |


# Theorems
## Reflexivity

- (question 18) - if $R$ reflexive, then $R\subseteq{R^2}$
- (question 20a) - if $R\subseteq{S}$ reflexive, then $S$ also reflexive
- (question 20b) - if $R$ reflexive, then ${R^2}$ also reflexive
- (question 20c) - $R$ reflexive, if and only if, $R^{-1}$ also reflexive 
- (question 20d) - if $R,S$ are reflexive, then $R\cap{S},R\cup{S}$ are reflexive
- (question 22) - if $R$ is irreflexive, then $S\subseteq{R}$ is also irreflexive

## Symmetry

- (question 23) - $R$ is symmetric if and only if $R^{-1} = R$ 
- (question 24) - composite of symmetric relations is symmetric
- (question 26) - if $R,S$ are symmetric, then $R\cap{S},R\cup{S}$ are symmetric
- (question 27) - let $R$ relation, then $R\cap{R}^{-1}$ and $R\cup{R}^{-1}$ are symmetric
- (defintion 2.10) - asymmetric implies antisymmetric
- (question 29) - asymmetry implies **irreflexivity**
- **Irreflexivity** and **transitivity** together imply asymmetry

## Transitivity

- (theorem 2.12) $R$ is transitive if and only if $R^2\subseteq{R}$
- (question 26) - if $R,S$ are transitive, then $R\cap{S}$ are also transitive

# Converse relation
converse relation $R^{-1}$, of a binary relation $R$, is the relation that occurs when the order of the elements is switched in the relation

- If a **relation** is reflexive, irreflexive, symmetric, antisymmetric, asymmetric, transitive, connected, trichotomous, a partial order, total order, strict weak order, total preorder (weak order), or an equivalence relation, **its converse is too**.
- Let $R$ relation from $A$ to $B$, and $S$ relation from $B$ to $C$, then $(RS)^{-1}=S^{-1}R^{-1}$. ^[Question 69]
- 

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
- The **equivalence class** of $a\in{A}$ under equivalence relation $R$ is the set $[a] = \{x \in A : x R a\}$
- The [[Bell numbers|Bell number]] $B_{n}$ counts **the number of different ways to partition a set** that has exactly $n$ elements, or equivalently, **the number of equivalence relations** on it.

## Partition of a set
 - A **partition of a set** (quotient set) is a grouping of its elements into non-empty subsets that called **cells** (equivalence classes), in such a way that every element is included in exactly one subset.
 - Every equivalence relation on a set defines a partition of this set, and every partition defines an equivalence relation.
 - A partition $P_1$ is called a **refinement** ^[עידון] of the partition $P_2$ if every set in $P_1$ is a subset of one of the sets in $P_2$.