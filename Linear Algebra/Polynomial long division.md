$$\frac{\color{blue}\text{dividend}}{\color{red}\text{divisor}}={{\color{red}\text{divisor}})\overline{\color{blue}\text{dividend}}}$$
___
${\color{green}\text{quotient}}:={0}$
${\color{orange}{\text{remainder}}}:={\color{blue}{\text{dividend}}}$

while r ≠ 0 and degree(r) ≥ degree(d) do

1. **D**ivide **the lead term** of the ${\color{orange}{\text{remainder}}}$ by **the lead term** of the ${\color{red}\text{divisor}}$.
	- Add the result to the $\color{green}\text{quotient}$. (above the bar)
2. **M**ultiply the ${\color{red}\text{divisor}}$ by the result just obtained.
	- Write the result under the first two terms of the dividend.
3. **S**ubtract the product just obtained from the appropriate terms of the ${\color{orange}{\text{remainder}}}$.
4. **B**ring down the next term from the dividend.

Repeat the previous three steps, except this time use the two terms that have just been written as the dividend.

The polynomial above the bar is the quotient, and the polynomial left over is the remainder.

$$\frac{\color{blue}\text{dividend}}{\color{red}\text{divisor}}={\color{green}\text{quotient}}+{\frac{\color{orange}{\text{remainder}}}{\color{red}\text{divisor}}}$$

## Pseudocode

The algorithm can be represented in pseudocode as follows, where +, −, and × represent polynomial arithmetic, and / represents simple division of two terms

```
function n / d is
    require d ≠ 0
    q ← 0
    r ← n             // At each step n = d × q + r

    while r ≠ 0 and degree(r) ≥ degree(d) do
        t ← lead(r) / lead(d)       // Divide the leading terms
        q ← q + t
        r ← r − t × d

    return (q, r)
```
