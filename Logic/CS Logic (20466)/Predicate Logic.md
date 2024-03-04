# Syntax

## Alphabet 

### Logical symbols

|                     | Logical symbols                                                      |
| ------------------- | -------------------------------------------------------------------- |
| Logical connectives | $\lnot,\rightarrow,\lor,\land,\leftrightarrow$                       |
| Punctuation Symbols | Comma and Parentheses                                                |
| Variables           | $v_{0},v_{1},v_{2},\dots$                                            |
| Quantifier symbols  | $∀$ (universal quantification), <br>$∃$ (existential quantification) |
| Equality            | $=$                                                                  |
### Non-logical symbols

|                   | Non-logical symbols                                               |
| ----------------- | ----------------------------------------------------------------- |
| Predicate Symbols | $P_{0}^{n}, P_{1}^{n},P_{2}^{n},\dots$ (For each arity $n\geq 0$) |
| Function Symbols  | $F_{0}^{n}, F_{1}^{n},F_{2}^{n},\dots$ (For each arity $n\geq 0$) |
| Constant Symbols  | $C_{0},C_{1},C_{2},\dots$                                         |
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
- *Quantifiers*. If φ is a formula and x is a variable, then $∀xφ$ (for all $x$, $φ$ holds) and $∃xφ$ (there exists $x$ such that $φ$) are formulas

Only expressions which can be obtained by finitely many applications of rules  are formulas. 

The formulas obtained from the first two rules are said to be **atomic formulas**.

#### Unique Readability

#todo 

#### Induction on wffs principle 

- (Theorem 5.4) 
	- Prove $H(A)$ for all atomic formulas A #todo 


### Free and bound variables 

#todo 

#### Sentence


#todo 

### substitution


# Semantic

