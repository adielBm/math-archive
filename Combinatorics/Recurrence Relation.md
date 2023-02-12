## The Characteristic Root Technique

Given a recurrence relation $a_n + \alpha a_{n-1} + \beta a_{n-2} = 0\text{,}$ the **characteristic polynomial** is
$$x^2 + \alpha x + \beta$$
giving the **characteristic equation**:
$$x^2 + \alpha x + \beta = 0.$$
then the solution to the recurrence relation is

- for **Distinct roots**: $a_n = ar_1^n + br_2^n$
- for **Repeated roots:** $a_n = ar^n + bnr^n$

where $a$ and $b$ are constants determined by the initial conditions of a recurrence relation.

___
$r=\frac{-b \pm \sqrt{b^2 - 4ac}}{2a}$

