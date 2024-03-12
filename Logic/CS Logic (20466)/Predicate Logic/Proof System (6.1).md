
Here we describe an example of a [[proof system]], which is [[Proof System#Strong completeness|complete]]
#  Characterization

#### Language

- Connectives $\{ \lnot,\to \}$
- Quantifier $\forall$

#### Axioms 

|                | Taulogical Axioms                                                          |                                          |
| -------------- | -------------------------------------------------------------------------- | ---------------------------------------- |
|                | $[\varphi\to(\psi\to \varphi)]$                                            |                                          |
|                | $[\varphi\to(\psi\to \theta)]\to[(\varphi\to \psi)\to(\varphi\to \theta)]$ |                                          |
| Contrapositive | $[(\lnot\varphi\to\lnot\psi)\to(\psi\to\varphi)]$                          |                                          |
|                | **Axioms of $\forall$**                                                    |                                          |
|                | $\forall x \varphi\to \varphi[t/x]$                                        | if no variable occur in $t$ become bonud |
|                | $\forall x(\varphi\to \psi)\to(\varphi\to \forall x\psi)$                  | if $x$ is not occur freely in $\varphi$  |

If it is first-order logic with equality, then we have also

|              | Equivalence                                                                                                                                                                                                   |
| ------------ | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| Reflexivity  | $\forall x (x = x)$                                                                                                                                                                                           |
| Symmetry     | $\forall x\forall y (x = y \rightarrow y = x)$                                                                                                                                                                |
| Transitivity | $\forall x \forall y \forall z (x = y \land y = z \rightarrow x = z)$                                                                                                                                         |
|              | (For each n-place function / prediacte symbol)                                                                                                                                                                |
|              | $\begin{align}\forall v_{0}\forall v_{1}\dots \forall_{2n-2}\forall_{2n-1}(((v_{0}=v_{n})\land\dots \land(v_{n-1}=v_{2n-1}))\to\\(F(v_{0},\dots,v_{n-1})=F(v_{n},\dots,v_{2n-1})))\end{align}$                |
|              | $\begin{align}\forall v_{0}\forall v_{1}\dots \forall_{2n-2}\forall_{2n-1}(((v_{0}=v_{n})\land\dots \land(v_{n-1}=v_{2n-1}))\to\\(P(v_{0},\dots,v_{n-1})\leftrightarrow P(v_{n},\dots,v_{2n-1})))\end{align}$ |

#### Rules of inference

- Universal generalization $\displaystyle\frac{\varphi}{\forall x\varphi}$
- Modus ponens $\displaystyle\frac{\varphi,(\varphi\to \psi)}{\psi}$

# Definitions

- A **theory** is a set of [[Predicate Logic#Free & Bound Variables|sentences]]
- Let $K$ be a theory, a **proof sequence from a theory** $K$ (in our calculus) is a sequence of formulas such that each formula in the sequence is either:
	- A logical axiom
	- A formula in the set $K$
	- Derived from two previous formulas in the sequence using one of the rules of inference

> **Note**: Here we restrict a theory to be set of *sentences*. but there are definitions with this restriction. Also, in a *proof sequence* (unlike to a *theory*), may be formulas that are *not* sentences.

# Theorems

- (6.1)
	- Let $\varphi$ be a proposition (of the propositional language) such that all of its elementary proposition are from $P_{1}, ..., P_{n}$. Let $\alpha_{1}, ..., \alpha_{n}$ be formulas of predicate logic, and let $\varphi'$ be the string obtained by replacing all occurrences of $P_{i}$  with $\alpha_{i}$, for $i=1, \dots, n$. Then:
		- $\varphi'$ is a formula of predicate logic.
		- If $M$ is a [[Semantic|model]] of the propositional language and $S$ is an [[Predicate Logic#Variable Assignment|assignment]] of predicate logic such that $M(P_{i}) = S(\alpha_{i})$ for all ${i}\leq n$, then $M(\varphi) = S(\varphi ')$
		- If $\varphi$ is a tautology, then $\varphi'$ is logically true
	- A formula obtained by systematic substitution in a tautology of formulas in place of elementary propositions is called a **tautology of predicate logic**, and according to (t6.1.c) it is logically true
- (6.2) Soundness Theorem
	- This proof system is [[Proof System#Soundness|sound]], i.e.
	- Let $K$ be a set of formulas and $\psi$ be a proposition. If $K\vdash \varphi$ (provable), then $K \models\varphi$ ([[Semantic#Logical Implication|logically implied]])
- 

