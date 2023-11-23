

- Propositional calculus (propositional logic)
	- **Proposition** (statement) - A declarative sentence that is either true or false, but not both. 
		- A statement is **atomic** if it cannot be divided into smaller statements, otherwise it is called **molecular**.
	- A **well-formed formula** (WFF) (Recursive definition):
		1. Any atomic statement is a WFF
		2. Any WFF preceded by $¬$ is a WFF
		3. Any two WFFs can be made into another WFF by writing one of these symbols between them, $∧, ∨, →, ↔$ and enclosing the result in parentheses
		4. Nothing else is a WFF
	- Logical connective



- **First-order logic (predicate logic)** - An extension of *propositional calculus* which permits quantifiers over elements
- Predicate







- **Alphabet** $\Sigma$ is a finite, nonempty set of elements called symbols (or letters)
- A **word** over an alphabet can be any finite sequence (i.e., string) of letters. 
	- Empty string (empty word) - $\epsilon$
- The set of all possible words over an alphabet $\Sigma$ is denoted by $\Sigma^*$
- **Language over Alphabet** $\mathcal{L}$
- The rules that specify when we can replace a string from $\Sigma^*$, the set of all strings of elements in the alphabet, with another string are called **the productions of the grammar**


- A phrase-structure grammar $G = (\Sigma, T, S, P)$ consists of an 
	- Alphabet $\Sigma$, 
	- A subset $T$ of $\Sigma$ consisting of terminal symbols
	- A start symbol S from $\Sigma$, 
	- A finite set of productions $P$. 
	- The set $\Sigma\setminus{T}$ is denoted by $N$. Elements of $N$ are called nonterminal symbols
	- Every production in $P$ must contain at least one nonterminal on its left side


> In some applications, especially in logic, the **alphabet** is also known as the **vocabulary** and **words** are known as **formulas** or **sentences**; this breaks the letter/word metaphor and replaces it by a word/sentence metaphor.




> #todo  Some of the elements of the vocabulary cannot be replaced by other symbols. These are called **terminals**, and the other members of the vocabulary, which can be replaced by other symbols, are called **nonterminals**.


- Formal language #todo  choose good definition!!!
	- A formal language can be identified with the set of formulas in the language.
	- A language $L$ is a possibly infinite set of strings over a finite alphabet $\Sigma$


-  #todo  (Grammar) $\set{V_{T}, V_N , S, R}$, where $V_T$ is the set of terminal elements, $V_N$ is the set of non-terminals, $S$ is a member of $V_N$, and $R$ is a finite set of rules







- Formal system
- Rule of inference
- Formal grammar


