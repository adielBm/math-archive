To prove that $\displaystyle\int_a^b f(x) \, dx = 0$, we'll use the given condition that in every subinterval of $[a,b]$, there exists a point where $f(x) = 0$. We'll prove this by contradiction.

Assume that $\displaystyle\int_a^b f(x) \, dx = A \neq 0$. Without loss of generality, let's assume $A > 0$ (if $A < 0$, we can simply consider $-f(x)$ instead of $f(x)$). 

Now, since $f(x)$ is integrable on $[a,b]$, by the properties provided in your notebook:

- From (1.27), $|f(x)|$ is also integrable on $[a,b]$.
- From (q1.50b), we have $\left|\int_a^b f(x) \, dx\right| \leq \int_a^b |f(x)| \, dx$.

Since $|f(x)| = |0| = 0$ wherever $f(x) = 0$, we can conclude that:

$$\int_a^b |f(x)| \, dx = 0$$

However, this contradicts $\displaystyle\int_a^b f(x) \, dx = A \neq 0$, because $\displaystyle\int_a^b |f(x)| \, dx = 0 < A$. 

Therefore, our assumption that $\displaystyle\int_a^b f(x) \, dx = A \neq 0$ must be false. Thus, $\displaystyle\int_a^b f(x) \, dx = 0$.