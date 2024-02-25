

- A **model** (or **interpretation**) of a language is a function $M$ from the elementary propositions set in to the set of two symbols $\{ \mathsf{T},\mathsf{F} \}$ that are called **truth values**
	- For each an elementary proposition $Q$, 
		- if $M(Q)=\mathsf{T}$ we say that $Q$ is **true** in the model $M$, and denote $M \models Q$
		- if $M(Q)=\mathsf{F}$ we say that $Q$ is **false** in the model $M$, and denote $M \not\models Q$
	- For each proposition $\varphi$,
		- If $\varphi$ is an elementary proposition, then $M(\varphi)$ is already defined
		- if $\varphi=\lnot{\psi}$ then $M(\varphi)=\begin{cases}\mathsf{T} & M(\psi)=\mathsf{F}\\ \mathsf{F} & M(\psi)=\mathsf{T} \end{cases}$
        - if $\varphi=(\psi \lor \theta)$ then $M(\varphi)=\begin{cases}\mathsf{T} & M(\psi)=\mathsf{T} \text{ or } M(\theta)=\mathsf{T}\\ \mathsf{F} & \text{otherwise} \end{cases}$
		- if $\varphi=(\psi \land \theta)$ then $M(\varphi)=\begin{cases}\mathsf{T} & M(\psi)=\mathsf{T} \text{ and } M(\theta)=\mathsf{T}\\ \mathsf{F} & \text{otherwise} \end{cases}$
		- if $\varphi=(\psi \rightarrow \theta)$ then $M(\varphi)=\begin{cases}\mathsf{T} & M(\psi)=\mathsf{F} \text{ or } M(\theta)=\mathsf{T}\\ \mathsf{F} & \text{otherwise} \end{cases}$
		- if $\varphi=(\psi \leftrightarrow \theta)$ then $M(\varphi)=\begin{cases}\mathsf{T} & (M(\psi)=\mathsf{T} \text{ and } M(\theta)=\mathsf{T}) \text{ or } (M(\psi)=\mathsf{F} \text{ and } M(\theta)=\mathsf{F})\\ \mathsf{F} & \text{otherwise} \end{cases}$
		- if $M(\varphi)=\mathsf{T}$ we say that $\varphi$ is **true** in the model $M$, and denote $M \models \varphi$
		- if $M(\varphi)=\mathsf{F}$ we say that $\varphi$ is **false** in the model $M$, and denote $M \not\models \varphi$
	- Let $K$ a set of propositions, $M$ is a **structure** (see §5.2.3), we say that $M$ is a **model** of $K$ and denote $M \models K$ if and only if every proposition in $K$ is true in $M$
		- If $K=\{ \varphi_{1},\dots ,\varphi_{n} \}$ is a finite set of propositions then $M \models K$ if and only if $M \models \varphi_{1}\land\dots\land\varphi_{n}$
	- In a language with $n$ elementary propositions there are $2^n$ models
	- (3.1, special-case of 2.5) Let $L_{1}$ and $L_{2}$ be proportional languages (possibly $L_{1}=L_{2}$), and let $\varphi$ be a proposition in both (and therefore the elementary propositions in $\varphi$ are in both languages). And let $M_{1}$ be a model of $L_{1}$ and $M_{2}$ be a model of $L_{2}$ such that for each elementary proposition $Q$ in $\varphi$ we have $M_{1}(Q)=M_{2}(Q)$ then $M_{1}(\varphi)=M_{2}(\varphi)$
	- (3.2) substitution of other proposition in subproposition with the the same truth value does not change the truth value of the proposition
	- A proposition $\varphi$ is a **tautology** (and denoted $\models \varphi$) if and only if it is true in every model in the language of the proposition. A proposition is a **contradiction** if and only if it is false in every model in the language of the proposition.
		- $\varphi$ is tautology if and only if $\lnot \varphi$ is contradiction
		- $\varphi$ is contradiction if and only if $\lnot \varphi$ is tautology
	- **Logical equivalence:** Propositions $\varphi$ and $\psi$ are **logically equivalent** (and denoted $\varphi \equiv \psi$) if and only if they are true in the same models exactly
		- Propositions are logically equivalent if and only if $\varphi\leftrightarrow{\psi}$ is a tautology
		- Propositions are logically equivalent if and only if they always have the same truth values
		- see [[Propositional Logic#Rules of Replacement (Logical Equivalences)]]
	- **Logical implication**: A propositions $\varphi$ **logically implies** a proposition $\psi$ (and $\psi$ **logically implied by** $\varphi$) if and only if in every model $M$, if $M\models{\varphi}$ then $M\models{\psi}$. We denote $\varphi \implies \psi$
		- $\varphi$ logically implies a proposition $\psi$ if and only if $\varphi\rightarrow{\psi}$ is a tautology. In other words, $\varphi \implies \psi$ if and only if $\models (\varphi\rightarrow{\psi})$
		- A set propositions $K$ **logically implies** a proposition $\psi$ (and $\psi$ **logically implied by** $K$) if and only if $\psi$ is true in every model in which all proposition in $K$ are true. We denote $K \implies \psi$
		- If $K=\{ \varphi_{1},\dots ,\varphi_{n} \}$ is a finite set of propositions, then, $K\implies \psi$ if and only if $\varphi_{1}\land\dots\land\varphi_{n}\implies \psi$. Hence, $\{ \varphi_{1},\dots ,\varphi_{n} \}\implies \psi$ if and only if $\models((\varphi_{1}\land\dots\land\varphi_{n})\to \psi)$
		- (3.6 **Compactness theorem**) if $K\implies \psi$ then there exists a finite subset $\{ \varphi_{1},\dots ,\varphi_{n} \}\subseteq K$ such that $\{ \varphi_{1},\dots ,\varphi_{n} \}\implies \psi$


## CNF & DNF

| Course Term             |                                                                             |                                                                                         |
| ----------------------- | --------------------------------------------------------------------------- | --------------------------------------------------------------------------------------- |
| קוניונקציה מרובה        | $\varphi_{1} \land\dots \land \varphi_{n}$                                  |                                                                                         |
| דיסיונקציה מרובה        | $\varphi_{1} \lor\dots \lor \varphi_{n}$                                    |                                                                                         |
| פסוק בסיסי              | $P$ or $\lnot P$                                                            | **Literal**<br>*Literal→¬Variable*<br>*Literal→Variable*<br>                            |
| קוניונקציה פשוטה        | קוניונקציה מרובה של פסוקים בסיסיים                                          | **Conjunction**<br>*Conjunction→Literal∧Conjunction*<br>*Conjunction→Literal*           |
| פסוק דיסיונקטיבי נורמלי | דיסיונקציה של קוניוקציות פשוטות                                             | **Disjunctive normal form (DNF)**<br>*DNF→(Conjunction)∨DNF*<br>*DNF→(Conjunction)*<br> |
| קוניונקציה פשוטה מלאה   | קוניונקציה פשוטה שמופיעה בה כל פסוק אלמנטרי (לחיוב או לשלילה) בדיוק פעם אחת | **Full Conjunction**                                                                    |



 
