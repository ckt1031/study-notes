## Proof Using Mathematical Induction

If $T(n) = rT(n-1) + a$, $T(0) = b$, and $r \neq 1$, then

$T(n) = r^n b + a \frac{1 - r^n}{1 - r}$

for all nonnegative integers $n$.

---

Basis: $f(0) = b$  
Inductive step: Assume $f(k) = rT(k -1) + a$  
Want to show $f(k + 1) = r^{k +1} b + a \frac{1 - r^{k+1}}{1 - r}$

$f(k+1) = rT(k) + a = r^2 T(k-1) + ra = r^3 T(k - 2) + ra + r^2 a$  
$= r^{k+1} T(k + 1 - 1) + a (r + r^2 + r^3 + \dots + r^{k +1}) = r^{k +1} b + a \frac{1 - r^{k+1}}{1 - r}$

By M.I., $T(n) = rT(n-1) + a = r^n b + a \frac{1 - r^n}{1 - r}$ is true for all nonnegative integers $n$.
