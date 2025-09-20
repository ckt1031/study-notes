## Inclusion-Exclusion Principle

![](https://www.youtube.com/watch?v=YlKDp03Kg68)

### One-to-One Functions

A one-to-one (injective) function from a set of size $n$ to a set of size $m$ requires that the size of $m$ be equal to or larger than the size of $n$. The number of such functions can be calculated as:

$m(m-1)(m-2)…(m-n+1)$

The $+1$ in $(m-n+1)$ ensures that the last element of the set of size $n$ has at least one element in the set of size $m$ to which it can be mapped.

### Onto Functions

An onto (surjective) function from a set of size $n$ to a set of size $m$ can be counted using the principle of inclusion-exclusion. The total number of onto functions is given by:

$m^n - \text{Number of non-onto functions} = \text{Number of onto functions}$

### Formula

${m \choose 1}(m-1)^n - {m \choose 2}(m-2)^n + {m \choose 3}(m-3)^n \dots {m \choose m}(m-m)^n$

$m^n - [{m \choose 1}(m-1)^n - {m \choose 2}(m-2)^n + {m \choose 3}(m-3)^n \dots {m \choose m}(m-m)^n]$

### Derangement

$$
\text{Derangement} = \text{All Possibilities} - \text{Not Derangement}
$$
$$
W (\text{Not Derangement}) = {n \choose 1} (n-1)!  - {n \choose 2} (n-2)!  + \cdots + (-1)^{p-1} {n \choose p} (n-p)! + \cdots
$$

### Formula of Derangement

$$D_n = n! \left[1 - \frac{1}{1!} + \frac{1}{2!} - \frac{1}{3!} + … (-1)^n \frac{1}{n!} \right]$$

### Probability

$$
\frac{D_n}{n!} = \left[ 1-\frac{1}{1!}+\frac{1}{2!}-\frac{1}{3!}+...+(-1)^{n}\frac{1}{n!} \right]
$$
