
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


> In some applications, especially in logic, the **alphabet** is also known as the **vocabulary** and **words** are known as **formulas** or **sentences**; this breaks the letter/word metaphor and replaces it by a word/sentence metaphor.




# Formal Language

- Formal language #todo  choose good definition!!!
	- A **formal language** can be identified with the set of formulas in the language.
	- A **formal language** $L$ is a possibly infinite set of strings over a finite alphabet $\Sigma$
	- A formal language is a language that is defined by a formal system.
	- Formal language, which is a set of well-formed formulas, which are strings of symbols from an alphabet, formed by a formal grammar (consisting of production rules or formation rules).
	- A **formal language** over an alphabet $\Sigma$ is a set of words over $\Sigma$. 
	- A **formal language** over $\Sigma$ is a subset of $\Sigma^*$

> The adjective *formal* is often omitted as redundant


- A **regular language** over $\Sigma$ is a formal language over $\Sigma$ which is accepted by some DFA.


- A **formal theory** is a set of sentences expressed in a formal language

# Formal System

- **Formal System** (also called a _logical calculus_, or a _logical system_)
	- A **formal system** (aka: *logical calculus*, *logical system*) is an abstract structure or formalization of an *axiomatic system* used for inferring theorems from axioms by a set of inference rules.
	- A **formal system** consists of a formal language together with a *deductive apparatus* (also called a _deductive system_).
	- A **formal system** is a formal language $L$ together with a deductive apparatus for $L$

A formal system is said to be recursive (i.e. effective) or recursively enumerable if the set of axioms and the set of inference rules are decidable sets or semidecidable sets, respectively.

> Although a formal language can be identified with its formulas, a formal system cannot be likewise identified by its theorems

# Deductive system

- A **deductive system**, (aka: *deductive apparatus*), consists of the axioms (or axiom schemata) and rules of inference that can be used to derive theorems of the system.
- The **deductive apparatus** may consist of a set of transformation rules, which may be interpreted as valid rules of inference, or a set of axioms, or have both.
- **Deductive system**, deductive apparatus, or proof system, which has rules of inference that take axioms and infers theorems, both of which are part of the formal language.

- A **deductive apparatus** for a formal language $\mathcal{L}$ is a formally specified system for deriving conclusions about the well-formed formulas of $\mathcal{L}$

- An example of deductive system is first order logic.

# Axiomatic System

- An **axiomatic system** is any set of axioms from which some or all axioms can be used in conjunction to logically derive theorems
	- An axiomatic system is said to be **consistent** if it lacks contradiction. 
	- A system is called **independent** if each of its underlying axioms is independent.
		- In an axiomatic system, an **axiom** is called **independent** if it cannot be proven or disproven from other axioms in the system.
	- An axiomatic system is called **complete** if for every statement, either itself or its negation is derivable from the system's axioms (equivalently, every statement is capable of being proven true or false)
	- An axiomatic system for which every model is isomorphic to another is called **categorial** (The property of categoriality ensures the completeness of a system, however the converse is not true)
- A **theory** is a consistent, relatively-self-contained body of knowledge which usually contains an axiomatic system and all its derived theorems.
- A **model** for an axiomatic system is a well-defined set, which assigns meaning for the undefined terms presented in the system, in a manner that is correct with the relations defined in the system. 
	- Two models are said to be **isomorphic** if a one-to-one correspondence can be found between their elements, in a manner that preserves their relationship

# Rule of inference

- A **rule of inference** is a logical form consisting of a function which takes premises, analyzes their syntax, and returns a conclusion (or conclusions).

# Formal grammar

-  #todo  (Grammar) $\set{V_{T}, V_N , S, R}$, where $V_T$ is the set of terminal elements, $V_N$ is the set of non-terminals, $S$ is a member of $V_N$, and $R$ is a finite set of rules


> #todo  Some of the elements of the vocabulary cannot be replaced by other symbols. These are called **terminals**, and the other members of the vocabulary, which can be replaced by other symbols, are called **nonterminals**.

## Unrestricted Grammar

An **unrestricted grammar** is a formal grammar $\displaystyle {\textstyle G=(N,T,P,S)}$, where

- $\displaystyle N$ is a finite set of nonterminal symbols,
- $\displaystyle T$ is a finite set of terminal symbols with $\displaystyle N$ and $\displaystyle T$ disjoint,
- $\displaystyle P$ is a finite set of production rules of the form $\displaystyle \alpha \to \beta$ , where $\displaystyle \alpha$ and $\displaystyle \beta$ are strings of symbols in $\displaystyle N\cup T$ and $\displaystyle \alpha$ is not the empty string, and
- $\displaystyle S\in N$ is a specially designated start symbol

As the name implies, there are no real restrictions on the types of production rules that unrestricted grammars can have.



## Context-sensitive Grammar (CSG)

- A **context-sensitive grammar** is a formal grammar in which the left-hand sides and right-hand sides of any production rules may be surrounded by a context of terminal and nonterminal symbols. 

## Context-Free Grammar (CFG)

- A **context-free grammar** is defined by $\displaystyle  G=(V,\Sigma ,R,S)$, where
	- $V$ is a finite set; each element $\displaystyle v\in V$ is called a **nonterminal character** or a variable. 
		- Each variable represents a different type of phrase or clause in the sentence. 
		- Variables are also sometimes called syntactic categories. 
		- Each variable defines a sub-language of the language defined by $G$.
	- $\Sigma$ is a finite set of **terminals**, disjoint from $V$, which make up the actual content of the sentence. The set of terminals is the alphabet of the language defined by the grammar $G$.
	- $R$ is a finite relation in $\displaystyle V\times (V\cup \Sigma )^{*}$, where the asterisk represents the Kleene star operation. 
		- The members of $R$ are called the (rewrite) rules or **productions of the grammar**. (also commonly symbolized by a $P$)
	- $S$ is the **start** variable (or start symbol), used to represent the whole sentence (or program). It must be an element of $V$.


- A phrase-structure grammar $G = (\Sigma, T, S, P)$ consists of an 
	- Alphabet $\Sigma$, 
	- A subset $T$ of $\Sigma$ consisting of **terminal** symbols
	- A **start** symbol S from $\Sigma$, 
	- A finite set of **productions** $P$. 
	- The set $\Sigma\setminus{T}$ is denoted by $N$. Elements of $N$ are called **nonterminal** symbols
	- Every production in $P$ must contain at least one nonterminal on its left side

- A **formal grammar** is defined as a set of production rules for such strings in a formal language.
- A **formal grammar** (consisting of production rules or formation rules).


- The rules that specify when we can replace a string from $\Sigma^*$, the set of all strings of elements in the alphabet, with another string are called **the productions of the grammar**

___

- **formation rules** are rules for describing which strings of symbols formed from the alphabet of a formal language are syntactically valid within the language.



- A **proof calculus** (or **proof system**) includes the components
	- Formal language: The set L of formulas admitted by the system, for example, propositional logic or first-order logic.
	- Rules of inference: List of rules that can be employed to prove theorems from axioms and theorems.
	- Axioms: Formulas in L assumed to be valid. All theorems are derived from axioms.


- Let L be a formal language. A **proof system** P for L comprises: Axioms and/or axiom schemata; Rules of inference for deriving theorems.
	- Also known as: axiom system, mathematical theory

- Formal Proof
