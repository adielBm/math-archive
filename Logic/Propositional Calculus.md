

- A compound proposition that is always true, no matter what the truth values of the propositional variables that occur in it, is called a **tautology** $\top$
	- Examples: $p\leftrightarrow{p},\quad p\rightarrow{p},\quad p\lor{(\lnot{p})},\quad p\rightarrow{T},\quad F\rightarrow{p}$
- A compound proposition that is always false is called a **contradiction**  $\bot$
	- Examples: $p\land\lnot{p}$
- A compound proposition that is neither a tautology nor a contradiction is called a **contingency**. 
	- Examples: $p\lor{q}$


- Negation of a tautology is always a contradiction
- Negation of a contradiction is always a tautology


- The compound propositions $p$ and $q$ are **logically equivalent** if $p\leftrightarrow{q}$ is a tautology. The notation $p \equiv q$ (or $p \dashv \vdash q$) denotes that $p$ and $q$ are logically equivalent. 

##  Logical Connectives (Logical Operator)

- Logical conjunction $\land$
- Logical disjunction $\lor$
- Logical Complement (Negation, Logical Not) $\lnot,\sim$
- Material Conditional (Material Implication) $\rightarrow \,,\supset$
	- $p\rightarrow{q}$ is true unless, $p$ is true and $q$ is false.

- Logical Consequence
	- **Syntactic consequence**: $\vdash$ (turnstile symbol)
	- **Semantic consequence**: $\models$

# Rules of Inferences

- Modus ponens (MP) (implication elimination)
	- $P \to Q,\; P\;\; \vdash\;\; Q$
- Syllogism
	- Disjunctive Syllogism (modus tollendo ponens (MTP))
		- $\displaystyle  P\lor Q,\lnot P\vdash Q$
	- Hypothetical Syllogism (transitivity, chain argument, chain rule)
		-  $(P \to Q) \land (Q \to R) \vdash P \to R$ 
- **Eliminations**
	- Biconditional Elimination
		- $\displaystyle  (P\leftrightarrow Q)\vdash (P\to Q)$
		- $\displaystyle  (P\leftrightarrow Q)\vdash (Q\to P)$
	- Conjunction Elimination (simplification)
		- $\displaystyle  (P\land Q)\vdash P$
		- $\displaystyle  (P\land Q)\vdash Q$
	- Disjunction Elimination (proof by cases, case analysis, *or* elimination) 
		- $\displaystyle  (P\to Q),(R\to Q),(P\lor R)\vdash Q$
- **Introductions**
	- Biconditional introduction
		- $\displaystyle  (P\to Q),(Q\to P)\vdash (P\leftrightarrow Q)$
	- Disjunction introduction (addition, *or* introduction)
		- $\displaystyle  P\vdash (P\lor Q)$
	- Conjunction introduction (conjunction, *and* introduction, adjunction)
		- $\displaystyle  P,Q\vdash P\land Q$
- Dilemma
	- Constructive dilemma
		- $\displaystyle  (P\to Q),(R\to S),(P\lor R)\vdash (Q\lor S)$
	- Destructive dilemma
		- $\displaystyle  (P\to Q),(R\to S),(\neg Q\lor \neg S)\vdash (\neg P\lor \neg R)$
- Modus Tollens (MT)
	- $\displaystyle  P\rightarrow Q,\neg Q  \therefore \neg P$
- Absorption
	- $\displaystyle  P\to Q\vdash P\to (P\land Q)$

- Tautology
	- $\displaystyle  P\lor P\vdash P$
	- $\displaystyle  P\land P\vdash P$


# Rules of Replacement (Logical Equivalences)

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
- Contraposition 
	- $p\rightarrow{q}\equiv{(\lnot{q})\rightarrow{(\lnot{p})}}$
- Exportation 
	- $p\rightarrow(q\rightarrow{r})\equiv{(p\land{q})\rightarrow{r}}$
- Negated conditionals
	-  $\lnot(p\rightarrow{q})\equiv{{p}\land(\lnot{q})}$
- Material implication 
	- $p\rightarrow{q}\equiv{\lnot{p}\lor{q}}$


- #todo   $p\leftrightarrow{q}\equiv{q\leftrightarrow{p}\equiv{(p\rightarrow{q})\land{(q\rightarrow{p})}\equiv{(p\land{q})\lor{((\lnot{p})\land{(\lnot{q})})}}}}$
- #todo  $((a\rightarrow{b})\rightarrow{c})\vdash(a\rightarrow({b}\rightarrow{c}))$
