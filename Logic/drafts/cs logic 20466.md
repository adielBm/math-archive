
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


 - The keyboard $\Sigma_{n}=\{ P_{1},\dots,P_{n},\lnot,\lor,\land,\rightarrow,\leftrightarrow,(,) \}$ is the **propositional keyboard** (המקלדת הפסוקית) 
- המקלדת המלאה
	 - The keyboard $\Sigma_{\infty}=\{ \lnot,\lor,\land,\rightarrow,\leftrightarrow,(,),P_{1},\dots,P_{n},\dots \}$
	 - Therefore, for all $n$ we have, $\Sigma_{n}\subset \Sigma_{n+1}\subset \Sigma_{\infty}$

- השפה הפסוקית המלאה 
	- הגדרה ברקורסיה
	- הגדרה מדורגת, אינדוקציה טבעית
		- $d(\varphi)$ is connective depth 


- Backus–Naur form (see section 2.12) #todo 
