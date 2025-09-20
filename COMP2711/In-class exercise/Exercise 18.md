Use Mathematical Induction to prove that:

---

If $S(n) = 2S(n-1)$ if $n \geq 1$ and $S(0) = 1$  
Then, $S(n) = 2^n$ for all $n \geq 0$

---

Basis: $S(1) = 2S(0) = 2$ since $2 \times 1 = 2$.  
Inductive step: $P(k) \to P(k+1)$ for every positive integer $k$.

Induction hypothesis $P(k)$:

$$2S(k - 1) = 2^k$$

So, assuming $P(k)$, it follows that:

$$S(k+1) = 2S(k) = 2 \cdot 2^k = 2^{k+1}$$

By principle of M.I., $P(k)$ is true for all integers $n \geq 0$.
