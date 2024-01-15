
- A **binary operation** on set $G$ is a function $*:G\times G\to G$

# Group

- A **group** is a set $G$ equipped with an operation $∗$ and a special element $e\in G$, called the **identity**, such that 
	- (i) the associative law holds: for every a, b, c ∈ G, a ∗ (b ∗ c) = (a ∗ b) ∗ c; 
	- (ii) $e ∗ a = a$ for all a ∈ G; 
	- (iii) for every a ∈ G, there is $a' ∈ G$ with $a' ∗ a = e$

### Abelian Group (Commutative Group)

- A group $G$ is called **abelian** if it satisfeis the commutative law: $x ∗ y = y ∗ x$ holds for every $x, y ∈ G$

## Group Homomorphism

- Given two groups, $(G, ∗)$ and $(H, ·)$, a **group homomorphism** from $(G, ∗)$ to $(H, ·)$ is a function $h : G → H$ such that for all $u$ and $v$ in $G$ it holds that $h(u∗v)=h(u)⋅h(v)$

- Types
	- Monomorphism - A group homomorphism that is **injective** (one-to-one)
	- Epimorphism - A group homomorphism that is **surjective** (onto)
	- Isomorphism - A group homomorphism that is **bijective** 
	- Endomorphism - A group homomorphism, $h: G → G$
	- Automorphism - A group endomorphism that is bijective, and hence an isomorphism