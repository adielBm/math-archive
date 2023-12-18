
## Propositional Equivalences 

- A compound proposition that is always true, no matter what the truth values of the propositional variables that occur in it, is called a **tautology** $\top$
	- Examples: $p\leftrightarrow{p},\quad p\rightarrow{p},\quad p\lor{(\lnot{p})},\quad p\rightarrow{T},\quad F\rightarrow{p}$
- A compound proposition that is always false is called a **contradiction**  $\bot$
	- Examples: $p\land\lnot{p}$
- A compound proposition that is neither a tautology nor a contradiction is called a **contingency**. 


- The compound propositions $p$ and $q$ are called **logically equivalent** if $p\leftrightarrow{q}$ is a tautology. The notation $p \equiv q$ denotes that $p$ and $q$ are logically equivalent. 


##  Logical Connectives (Logical Operator)

- Logical conjunction $\land$
- Logical disjunction $\lor$
- logical complement (Negation) $\lnot$

- Material conditional $\rightarrow$
	- $p\rightarrow{q}$ is true unless, $p$ is true and $q$ is false.
	- Contraposition: $p\rightarrow{q}\equiv{(\lnot{q})\rightarrow{(\lnot{p})}}$
	- Import–export: $p\rightarrow(q\rightarrow{r})\equiv{(p\land{q})\rightarrow{r}}$
	-  $p\rightarrow{q}\equiv{\lnot({p}\land(\lnot{q}))}$
	- Material implication $p\rightarrow{q}\equiv{\lnot{p}\lor{q}}$
	- Transitivity: $(p \to q) \land (q \to r) \models p \to r$


>***Tautology** is Negation of Contradiction. 
>**Contradiction** is Negation of Tautology.*

## Logical Equivalences

- Double negation law 
	- $\lnot\lnot{p}\equiv{p}$
- Commutativity
	- (AND) $p\land{q}\equiv{q\land{p}}$
	- (OR) $p\lor{q}\equiv{q\lor{p}}$
- Associativity 
	- (AND) $(p\land{q})\land{r}\equiv{p\land({q}\land{r})}$
	- (OR) $(p\lor{q})\lor{r}\equiv{p\lor({q}\lor{r})}$
- Distributivity 
	- (OR over AND): $({p\lor({q\land{r}})})\equiv({({p\lor{q}})\land({p\lor{r}})})$
	- (AND over OR): $({p\land({q\lor{r}})})\equiv({({p\land{q}})\lor({p\land{r}})})$
- De Morgan's laws
	- $\lnot{(p\land{q})}\equiv{(\lnot{p})\lor{(\lnot{q})}}$
	- $\lnot{(p\lor{q})}\equiv{(\lnot{p})\land{(\lnot{q})}}$
- Identity laws
	- $p\land{T}\equiv{p}$
	- $p\lor{F}\equiv{p}$
- Domination laws 
	- $p\lor{T}\equiv{T}$
	- $p\land{F}\equiv{F}$
- Idempotency 
	- (AND): $p\land{p}\equiv{p}$
	- (OR): $p\lor{p}\equiv{p}$
- Absorption laws 
	- $p\lor d$







- $\lnot\forall{x(p(x))\equiv{\exists{x(\lnot{p(x)})}}}$
- $\lnot\exists{x(p(x))\equiv{\forall{x(\lnot{p(x)})}}}$
- $\forall{x(p(x))\equiv{\lnot\exists{x(\lnot{p(x)})}}}$
- $p\leftrightarrow{q}\equiv{q\leftrightarrow{p}\equiv{(p\rightarrow{q})\land{(q\rightarrow{p})}\equiv{(p\land{q})\lor{((\lnot{p})\land{(\lnot{q})})}}}}$

## Logical consequence 


- **Syntactic consequence**: $\vdash$
- **Semantic consequence**: $\models$




- Modus ponens (MP)
	- $P \to Q,\; P\;\; \vdash\;\; Q$
- Modus tollens (MT)
	- $\displaystyle  P\rightarrow Q,\neg Q  \therefore \neg P$

- $((a\rightarrow{b})\rightarrow{c})\vdash(a\rightarrow({b}\rightarrow{c}))$
