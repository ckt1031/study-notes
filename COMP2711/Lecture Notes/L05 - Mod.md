## Modular

$a | b$ means that **a divides b**, if it is true, then $b/a$ is an integer.

## Divisibility

if $a|b$ and $a|c$, then $a|(b+c)$

## Euclid's Division Theorem

For any integer $a$ and any positive integer $d$, there exist unique integers $q$ and $r$ such that:

$$𝑎 = 𝑑 𝑞 + 𝑟$$

- $d$: divisor
- $q$: quotient
- $r$: remainder

## Proof of Uniqueness

Assume that $a = dq_1 + r_1$ and $a = dq_2 + r_2$

Then $dq_1 + r_1 = dq_2 + r_2$

$d(q_1 - q_2) = r_2 - r_1$

So, $d | r_2 - r_1$

Since $0 \leq r_1 < d$ and $0 \leq r_2 < d$, then $-d < r_2 - r_1 < d$

$d | r_2 - r_1$ and $0 \leq r_1 < d$ and $0 \leq r_2 < d$

Therefore, $r_2 - r_1 = 0$, so $r_1 = r_2$, and $q_1 = q_2$.

## Modular Arithmetic

$$a\equiv b \ (\text{mod} \ m)$$

$$(a+b) \text{ mod } m = ((a \text{ mod } m) + (b \text{ mod } m)) \text{ mod } m $$

$$(a + b) \text{ mod } m = (a + (b \text{ mod } m)) \text{ mod } m$$

$$(a + b) \text{ mod } m = ((a \text{ mod } m) + b) \text{ mod } m$$

$$(a \cdot b) \text{ mod } m = (a \cdot (b \text{ mod } m)) \text{ mod } m$$

$$(a \cdot b) \text{ mod } m = ((a \text{ mod } m) \cdot b) \text{ mod } m$$

## Associativity

$$a +_m (b +_m c) = (a +_m b) +_m c$$

## Congruences

If $a \equiv b \ (\text{mod} \ m)$ and $c \equiv d \ (\text{mod} \ m)$, then:

$$
a + c \equiv b + d \ (\text{mod} \ m)
$$

$$
a c \equiv b d \ (\text{mod} \ m)
$$

$$a \equiv b \ (\text{mod} \ m) \Rightarrow m | (a - b)$$

$$c \equiv d \ (\text{mod} \ m) \Rightarrow m | (c - d)$$

$$a + c \equiv b + d \ (\text{mod} \ m) \Rightarrow m | ((a + c) - (b + d))$$

> We can also use minus sign to represent the congruence, for example:  
> $a - c \equiv b - d \ (\text{mod} \ m)$

> [!Example 1]-
>
> $7 \equiv 1 \ (\text{mod} \ 5)$, $11 \equiv 1 \ (\text{mod} \ 5)$
>
> $7 + 11 \equiv 1 + 1 \ (\text{mod} \ 5)$
