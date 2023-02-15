## Material conditional $\rightarrow$
$p\rightarrow{q}$ is true unless, $p$ is true and $q$ is false.

- Contraposition: $p\rightarrow{q}\equiv{(\lnot{q})\rightarrow{(\lnot{p})}}$
- Import–export: $p\rightarrow(q\rightarrow{r})\equiv{(p\land{q})\rightarrow{r}}$
- $p\rightarrow{q}\equiv{\lnot({p}\land(\lnot{q}))}\equiv{(\lnot{p}\lor{q})}$
- Transitivity: $(p \to q) \land (q \to r) \models p \to r$
## Tautology $\top$
- $p\leftrightarrow{p}$
- $p\rightarrow{p}$
- $p\lor{(\lnot{p})}$
- $p\rightarrow{T}$
- $F\rightarrow{p}$
## Contradiction $\bot$
- $p\land\lnot{p}$

>***Tautology** is Negation of Contradiction. 
>**Contradiction** is Negation of Tautology.*

## Logical equivalence (1.2)
- $\lnot\lnot{p}\equiv{p}$
- Commutativity (AND) $p\land{q}\equiv{q\land{p}}$
- Commutativity (OR) $p\lor{q}\equiv{q\lor{p}}$
- Associativity (AND): $(p\land{q})\land{r}\equiv{p\land({q}\land{r})}$
- Associativity (OR): $(p\lor{q})\lor{r}\equiv{p\lor({q}\lor{r})}$
- Distributivity (OR over AND): $({p\lor({q\land{r}})})\equiv({({p\lor{q}})\land({p\lor{r}})})$
- Distributivity (AND over OR): $({p\land({q\lor{r}})})\equiv({({p\land{q}})\lor({p\land{r}})})$
- De Morgan's laws: $\lnot{(p\land{q})}\equiv{(\lnot{p})\lor{(\lnot{q})}}$
- De Morgan's laws: $\lnot{(p\lor{q})}\equiv{(\lnot{p})\land{(\lnot{q})}}$
- $p\land{T}\equiv{p}$
- $p\lor{F}\equiv{p}$
- $p\lor{T}\equiv{T}$
- $p\land{F}\equiv{F}$
- Idempotency (AND): $p\land{p}\equiv{p}$
- Idempotency (OR): $p\lor{p}\equiv{p}$
- $\lnot\forall{x(p(x))\equiv{\exists{x(\lnot{p(x)})}}}$
- $\lnot\exists{x(p(x))\equiv{\forall{x(\lnot{p(x)})}}}$
- $\forall{x(p(x))\equiv{\lnot\exists{x(\lnot{p(x)})}}}$
- $p\leftrightarrow{q}\equiv{q\leftrightarrow{p}\equiv{(p\rightarrow{q})\land{(q\rightarrow{p})}\equiv{(p\land{q})\lor{((\lnot{p})\land{(\lnot{q})})}}}}$

## Logical consequence 
#### (Defintion 3)

#### Theorem (5)
- 
#### Theorem (6)
- ***Modus ponens***: $P \to Q,\; P\;\; \vdash\;\; Q$

___
more (not appear in the book)
- $((a\rightarrow{b})\rightarrow{c})\vdash(a\rightarrow({b}\rightarrow{c}))$
