
- A **formal proof** (סדרת הוכחה פורמלית) of a given proposition $\varphi$ is a finite sequence of propositions such that $\varphi$ is the last in the sequence, and each proposition in the sequence is either axiom or derived from the previous propositions in the sequence.
- A **proof calculus** (תחשיב, or **proof system**)

## Hilbert calculus

- A **Hilbert calculus** (תחשיב הילברט, or **Hilbert system**) 
	- A set of propositions that will be called the **logical axioms** (אקסיומות לוגיות) of the calculus. 
		- Naturally, these should be propositions whose truth we trust, but it is equally important that they be useful. The selection of axioms is not a process of discovering everything that is certainly true, but rather a process of identifying the facts that are clearly likely to be helpful in proving additional facts.
	- A set of rules, which will be called the **inference rules** (כללי גזירה) of the calculus. 
		- If we accept as proven several propositions, called the **assumptions** (הנחות), then according to the inference rules, we are allowed to add an additional proposition to the proven claims, which will be called the **conclusion** (מסקנה)



- A **proof sequence** (סדרת הוכחה) is a finite sequence of propositions in which each proposition is either a logical axiom or derived from propositions that appeared before it in the sequence through inference rules. (Typically, we think of the proof sequence as proving the last proposition appearing in the sequence, and we say it is a proof sequence for that proposition.) 
- A proposition that has a proof sequence is called a **provable** (יכיח) proposition in the calculus.


##### Example of Hilbert calculus

- **Our calculus** is an example of Hilbert calculus:
	- Language: The dialect $L_{\rightarrow }$ of the proposional language 
		- convectives: $\{ \lnot,\rightarrow \}$
		- the propositions are either elementary propositions, negation propositions in the form $\lnot{\varphi}$, or propositions in the form $(\varphi\rightarrow \psi)$
	- Axioms: (Each one is general form of one of infinite propositions. Also, these axioms are tautologies (q4.6))
		- $(\varphi\rightarrow (\psi\rightarrow \varphi))$
		- $([\varphi\rightarrow (\psi\rightarrow \theta)]\rightarrow [(\varphi\rightarrow \psi)\rightarrow (\psi\rightarrow \theta)])$
		- $[(\lnot \varphi\rightarrow \lnot\psi )\rightarrow (\psi\rightarrow \varphi)]$
	- Inference rules (actually one here)
		- Modus ponens $\displaystyle\frac{\varphi,(\varphi \rightarrow \psi)}{\psi}$

- Definitions for our calculus:
	- Let $K$ be a set of propositions, a **proof sequence from a set** $K$ (in our calculus) is a sequence of propositions $\varphi_{1},\dots,\varphi_{n}$ such that each proposition in the sequence is either: 
		- A logical axiom
		- A proposition in the set $K$
		- Derived from two previous propositions in the sequence using modus ponens
	- A **proof sequence in the calculus** is proof sequence from the empty set. (i.e. each proposition is either a logical axiom or derived from two previous propositions)
	- A **proof sequence from $K$ to** $\varphi$ is a proof sequence from $K$, such that $\varphi$ is the last proposition
	- $\varphi$ is **theorem** of $K$ if and only if it has (at least one) proof sequence from $K$. we denote $K \vdash \varphi$


- (theorem 4.2)
	- If $\varphi_{1},\dots,\varphi_{n}$ is a proof sequence from $K$, then for each $i\leq n$ the proof sequence $\varphi_{1},\dots,\varphi_{i}$ is is a proof sequence from $K$. ( #todo )
	- If $\varphi_{1},\dots,\varphi_{n}$ is a proof sequence from $K$, and $\psi_{1},\dots,\psi_{n}$ is also a proof sequence from $K$, then  $\varphi_{1},\dots,\varphi_{n},\psi_{1},\dots,\psi_{n}$
	- If $K\vdash \varphi$ and $K \subseteq K'$ then $K' \vdash \varphi$
	- If $\varphi$ is a theorem of $K$, and $K \cup \{ \varphi \}\vdash \psi$ then $K \vdash \psi$. 
		- Similarly, $\varphi_{1},\dots,\varphi_{n}$ are theorems of $K$ and $K\cup \{ \varphi_{1},\dots,\varphi_{n} \}\vdash \psi$ then $K\vdash \psi$.
	- If $K \vdash \varphi$ then there exists a finite subset of $K'$ such that $K' \vdash \varphi$


___

# other 



- Let L be a formal language. A **proof system** P for L comprises: Axioms and/or axiom schemata; Rules of inference for deriving theorems.
	- Also known as: axiom system, mathematical theory
- Formal Proof
- **formation rules** are rules for describing which strings of symbols formed from the alphabet of a formal language are syntactically valid within the language.


- A proof system is **complete** if every valid formula is provable
- A proof system is **sound** if every provable formula is valid

