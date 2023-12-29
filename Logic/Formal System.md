
# Rule of inference

- A **rule of inference** is a logical form consisting of a function which takes premises, analyzes their syntax, and returns a conclusion (or conclusions).

# Formal System

- **Formal System** (aka: _logical calculus_, _logical system_)
	- A **formal system** is an abstract structure or formalization of an *axiomatic system* used for inferring theorems from axioms by a set of inference rules.
	- A **formal system** consists of a formal language together with a *deductive apparatus* (also called a _deductive system_).
	- A **formal system** is a formal language $L$ together with a deductive apparatus for $L$


- A formal system is **sound** if and only if every well-formed formula that can be proven in the system is logically valid with respect to the logical semantics of the system.
- A formal system is **recursive** (i.e. effective) or recursively enumerable if the set of axioms and the set of inference rules are decidable sets or semidecidable sets, respectively.

> Although a formal language can be identified with its formulas, a formal system cannot be likewise identified by its theorems

# Deductive system

- A **deductive system**, (aka: *deductive apparatus*), consists of the axioms (or axiom schemata) and rules of inference that can be used to derive theorems of the system.
- The **deductive apparatus** may consist of a set of transformation rules, which may be interpreted as valid rules of inference, or a set of axioms, or have both.
- **Deductive system**, deductive apparatus, or proof system, which has rules of inference that take axioms and infers theorems, both of which are part of the formal language.

- A **deductive apparatus** for a formal language $\mathcal{L}$ is a formally specified system for deriving conclusions about the well-formed formulas of $\mathcal{L}$

- An example of deductive system is first order logic.

# Axiomatic System