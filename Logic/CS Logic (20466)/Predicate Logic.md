# Syntax

## Alphabet 

The alphabet of a first-order language consists of the following distinct symbols:
### Logical symbols

|                            | Logical symbols                                                      |
| -------------------------- | -------------------------------------------------------------------- |
| Logical connectives        | $\lnot,\rightarrow,\lor,\land,\leftrightarrow$                       |
| Punctuation Symbols        | Comma and Parentheses                                                |
| Variables ($\mathrm{VAR}$) | $v_{0},v_{1},v_{2},\dots$                                            |
| Quantifier symbols         | $∀$ (universal quantification), <br>$∃$ (existential quantification) |
| Equality (optional)        | $=$                                                                  |
### Non-logical symbols

|                             | Non-logical symbols                                               |
| --------------------------- | ----------------------------------------------------------------- |
| Predicate Symbols           | $P_{0}^{n}, P_{1}^{n},P_{2}^{n},\dots$ (For each arity $n\geq 0$) |
| Function Symbols (optional) | $F_{0}^{n}, F_{1}^{n},F_{2}^{n},\dots$ (For each arity $n\geq 0$) |
| Constant Symbols (optional) | $C_{0},C_{1},C_{2},\dots$                                         |
## Language

### Terms

The set of terms is inductively defined by the following rules:

- Each variable and each constant symbol is a **term**
- If $F$ is an $n$-ary function symbol, and $t_{1},\dots, t_{n}$ are terms, then $F(t_{1},\dots,t_{n})$ is a term
### Formulas

The set of **formulas** (also called **well-formed formulas** or **WFFs**) is inductively defined by the following rules:

- *Predicate symbols*. If $P$ is an $n$-ary predicate symbol and $t_{1}, \dots, t_{n}$ are terms then $P(t_{1},\dots,t_{n})$ is a formula. 
- *Negation*. If $φ$ is a formula, then $¬ φ$ is a formula. 
- *Binary connectives*. If $φ$ and $ψ$ are formulas, then $( φ → ψ )$ is a formula. (Similar rules apply to other binary logical connectives). 
- *Quantifiers*. If φ is a formula and $x$ is a variable, then $∀xφ$ (for all $x$, $φ$ holds) and $∃xφ$ (there exists $x$ such that $φ$) are formulas

Only expressions which can be obtained by finitely many applications of rules  are formulas. 

The formulas obtained from the first two rules are said to be **atomic formulas**.

#### Unique Readability

#todo 

#### Induction on wffs principle 

- (Theorem 5.4) 
	- Prove $H(A)$ for all atomic formulas A #todo 


### Free & Bound Variables

- For any quantifier $Q$, and let be a formula $QxB$, we say that $B$ is the **scope** of $Qx$
- The concept that a variable $x$ **occurs free** or **bound** (also: $x$ is a **free** or **bound occurrence**) in formula is defined recursively as follows:
	- Atomic formulas:
		- If $φ$ is an atomic formula, then $x$ occurs free in $φ$ if and only if $x$ occurs in $φ$. 
		- Moreover, there are no bound variables in any atomic formula.
	- Negation:
		- $x$ occurs free in $¬φ$ if and only if $x$ occurs free in φ. 
		- $x$ occurs bound in $¬φ$ if and only if $x$ occurs bound in φ
	- Binary connectives:
		- $x$ occurs free in $(φ → ψ)$ if and only if $x$ occurs free in either $φ$ or $ψ$. 
		- $x$ occurs bound in $(φ → ψ)$ if and only if $x$ occurs bound in either $φ$ or $ψ$. 
		- (The same rule applies to any other binary connective in place of $→$.)
	- Quantifiers: ($Q$ is $\forall$ or $\exists$)
		- $x$ occurs free in $Qyφ$, if and only if $x$ occurs free in $φ$ and $x$ is a different symbol from $y$. 
		- $x$ occurs bound in $Qyφ$, if and only if $x$ is $y$ or $x$ occurs bound in $φ$. 

- A variable $x$ is a **free variable** in $φ$, if and only if, it has at least one free occurrence in $\varphi$ 
- A variable $x$ is a **bound variable** in $φ$, if and only if, all occurrences of $x$ in $φ$ are bound
- A formula $\varphi$ is called a **sentence**, if these is no free variable in $\varphi$, i.e. all occurrences of $x$ in $φ$ are bound

### Substitution

- The **substitution** $\varphi[t/x]$ replaces each free occurrence of the variable $x$ in the formula $\varphi$ with the term $t$
- The substitution $\varphi[t/x]$ is a **capture-avoiding substitution** if and only if no variable occur in $t$ become bonud (we say that $t$ is **substitutable** for $x$ in $\varphi$, or the quantifier $Qx$ does not **capture** the variable $x$ in $t$.)

# Semantic

## Structure (Model)

- A **model** or **structure** $M = \langle A; c_1^M, \ldots; F_1^M, \ldots ;P_{1}^{M},\dots\rangle$ is defined as
	- $A$ is a non-empty set called the **domain** ($A$ is sometimes denoted by $|M|$)
	- **Interpretation Function** $I$ mapping non-logical symbols for predicates, functions, and constants.
		- For each constant symbol $c$, assigns a member $c^M$ of the domain $A$
		- For each each $n$-ary predicate symbol $P$, assigns an $n$-place relation $P^M\subseteq A^n$
		- For each each $n$-ary function symbol $F$, assigns an $n$-ary function $F^{M}: A^{n}\to{A}$. 


> If we don't mention other, we are in **first-order logic with equality**, which means, the equality symbol ̇$=$ is defined as the identity relation $R = \{(x, x) : x \in A\}$


#### Variable Assignment

- A **(variable) assignment** for a structure $M$ with the domain $A$ is a mapping $S:\text{dom}(S)\to A$ where $\text{dom}(S)\subseteq{VAR}$
	- A **(variable) assignment** for a formula $\varphi$ is a mapping $S:\text{dom}(S)\to A$ where $V(\varphi)\subseteq\text{dom}(S)\subseteq{VAR}$ and $V(\varphi)$ is the set of variables which occur freely in $\varphi$
		- If $\varphi$ is a sentence, then every assignment is *for a formula* $\varphi$, because $V(\varphi)=\emptyset$
	- If $S$ is an assignment for a structure $M$, and $x \in \text{VAR}$, and $a\in{A}$ we denote $S\langle{x|a}\rangle$ if $S(x)=a$

### Truth Value

Given structure $M$, and an assignment $S$ for a formula $\varphi$.

- If $\varphi$ is an atomic formula $P(t_{1},\dots,t_{n})$, then $\varphi$ is **true** if $(t_{1}^S,\dots,t_{n}^S)\in{P^M}$, otherwise $\varphi$ is **false**
- If $\varphi$ is the formula $\lnot{\psi}$, then $\varphi$ is **true** if is $\psi$ is false, otherwise $\varphi$ is **false**. (similar way for the other connectives as in as in propositional logic)
- If $\varphi$ is the formula $\exists x\psi$ then $\varphi$ is **true** if and only if there exists an element $a\in A$ such that $\psi$ is true in $S\langle{x|a}\rangle$
- If $\varphi$ is the formula $\forall x\psi$ then $\varphi$ is **true** if and only if for each element $a\in A$ the formula $\psi$ is true in $S\langle{x|a}\rangle$
- The **truth value** of a formula is **truth** if it is true, and **falsity**
- Notaion: if $\varphi$ is true we can denote $S(\varphi)=\mathsf{T}$ or $S\models{\varphi}$ or $M\models_{S}\varphi$. If $\varphi$ is false we denote $S(\varphi)=\mathsf{F}$ or $S\nvDash\varphi$ or $M\nvDash_{S}\varphi$.

## Prenex normal form (5.7.2)