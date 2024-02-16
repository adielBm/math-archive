
| Terms |  |  |
| ---- | ---- | ---- |
| Relational Structures |  | מבני יחסים, מבנים |
|  |  | עצי הצגה |
|  |  | אינדוקציה מבנית (הוכחה, הגדרה) |
| Many sorted logic |  | לוגיקה רב סוגית |
| Temporal logic |  | לוגיקת זמן |
|  |  | אימות תכניות |
| Modal logic |  | לוגיקה מודאלית |
|  |  | לוגיקה מסדר שני |
|  |  | המקלדת $\Sigma_{n}$ |
| Homogeneous relation, endorelation |  |  |


- Any finite or infinite set $\Sigma$ of letters (arbitrary symbols) is called an **alphabet** or **keyboard**. 

- The set of strings, (i.e., finite sequences of letters), is called the set of words over $\Sigma$, denoted by $\Sigma^*$. 
- In $\Sigma^*$, the **concatenation** (symbol $\cdot$) binary operation is defined. 
	- $α⋅β$ or $\alpha \beta$ is the string composed of the concatenation of $α$ and $β$. Its beginning is the string $α$, and its continuation is the string β. 
	- If a word can be written as $α⋅β$, then $α$ is the **prefix** of the word, and $β$ is its **suffix**.
- Empty string $\varepsilon \in\Sigma^*$
- Every subset $L\subseteq \Sigma^*$ is a **language over** $\Sigma$

- Unary connective (קשר חד-מקומי): $\lnot$
- Binary connective (קשר דו-מקומי): $\lor,\land,\rightarrow,\leftrightarrow$. (notation: we use in $@$ for any binary connective)
- $n$-ary connective (קשר $n$-מקומי): $\lor,\land,\rightarrow,\leftrightarrow$

 - The keyboard $\Sigma_{n}=\{ P_{1},\dots,P_{n},\lnot,\lor,\land,\rightarrow,\leftrightarrow,(,) \}$ is the **propositional keyboard** (המקלדת הפסוקית) 
- המקלדת המלאה
	 - The keyboard $\Sigma_{\infty}=\{ \lnot,\lor,\land,\rightarrow,\leftrightarrow,(,),P_{1},\dots,P_{n},\dots \}$
	 - Therefore, for all $n$ we have, $\Sigma_{n}\subset \Sigma_{n+1}\subset \Sigma_{\infty}$


- השפה הפסוקית (המלאה) 
	- Recursive definition (הגדרה ברקורסיה)
		- Any (מחרוזת) with one symbol (סימן) that is an elementary proposition is a proposition
		- Any proposition preceded by $¬$ is a proposition
		- Any two propositions can be made into another proposition by writing one of these symbols between them, $∧, ∨, →, ↔$ and enclosing the result in parentheses
	- הגדרה מדורגת, אינדוקציה טבעית
		- $E_{0}$ is the set of of elementary propositions with one symbol
		- Given $E_{n+1}$ is defined: $E_{n}$ is the set of all strings in $E_{n+1}$ in additional all strings $(\varphi\land\psi)$, $(\varphi\lor\psi)$, $(\varphi\rightarrow\psi)$, and $(\varphi\leftrightarrow\psi)$ for which $\psi$ and $\varphi$ are in $E_{n-1}$
		- A string is called a **proposition** if and only if, it's in one of the sets $E_{n}$ 
		- The (העומק הקשרי, הדרגה) of a proposition $\varphi$ which denote $d(\varphi)$ is the smallest number $n$ such that $\varphi\in E_{n}$
			- A proposition $\varphi$ is an elementary proposition, if and only if, $d(\varphi)=0$



- Theorem 2.1
	- Let $\mathbf{R}$ be a property of some (or all) the strings. Given:
		- Every elementary proposition has the property $\mathbf{R}$
		- If a proposition $\varphi$ has the property $\mathbf{R}$ then $\lnot\varphi$ has the property $\mathbf{R}$ as well
		- For each binary connective @, if $\varphi$ and $\psi$ has the property $\mathbf{R}$, then $(\varphi{@}\psi)$ has the property $\mathbf{R}$ as well
	- Then, every proposition has the property $\mathbf{R}$
	

- Backus–Naur form (see section 2.12) #todo 
