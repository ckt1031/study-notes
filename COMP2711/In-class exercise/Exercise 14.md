## Question

Using Extended GCD algorithm to find the integers $x$ and $y$, such that $\gcd(57,81) = x \cdot 57 + y \cdot 81$.

---

$$81 = 57 \cdot 1 + 24$$

$$57 = 24 \cdot 2 + 9$$

$$24 = 9 \cdot 2 + 6$$

$$9 = 6 \cdot 1 + 3$$

$$6 = 3 \cdot 2 + 0$$

$$\gcd(57,81) = 3$$

By Using the Extended Euclidean Algorithm

$$3 = 9 - 6 \cdot 1$$

$$3 = 9 - (24 - 9 \cdot 2) = 9 \cdot 3 - 24$$

$$3 = (57 - 24 \cdot 2) \cdot 3 - 24 = 57 \cdot 3 - 24 \cdot 7$$

$$3 = 57 \cdot 3 - (81 - 57 \cdot 1) \cdot 7 = 57 \cdot 10 - 81 \cdot 7$$

So, $x = 10, y = -7$
