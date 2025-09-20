## Definition

An infinite sequence is an ordered list of real numbers: $a_1, a_2, …, a_n, …$

Can be viewed as a function $f$ with domain $\{1, 2, 3, …\}$ where $f(n) = a_n$.

## Limit of an Infinite Sequence

* Studies the trending behavior of sequence members as $n \to \infty$, denoted by $\lim_{n \to \infty} a_n$.
* $\lim_{n \to \infty} a_n = L$ (where L is a finite number) means the sequence values get arbitrarily close to L as $n$ increases.
* **Possibilities for the limit:**
	* **L (a finite value):** The limit exists.
	* **$\infty$ or $-\infty$:** The limit does not exist (divergent).
	* **Does not exist (oscillation):** The sequence values don't approach a single value.

## Limit Laws for Infinite Sequences

Assume $\lim_{n \to \infty} a_n$ and $\lim_{n \to \infty} b_n$ exist.

* $\lim_{n \to \infty} (a_n + b_n) = \lim_{n \to \infty} a_n + \lim_{n \to \infty} b_n$
* $\lim_{n \to \infty} (a_n - b_n) = \lim_{n \to \infty} a_n - \lim_{n \to \infty} b_n$
* $\lim_{n \to \infty} (a_n b_n) = (\lim_{n \to \infty} a_n) \cdot (\lim_{n \to \infty} b_n)$
* $\lim_{n \to \infty} \frac{a_n}{b_n} = \frac{\lim_{n \to \infty} a_n}{\lim_{n \to \infty} b_n}$ (if $\lim_{n \to \infty} b_n \neq 0$)
* $\lim_{n \to \infty} (a_n)^p = (\lim_{n \to \infty} a_n)^p$ (if $p > 0$ and $a_n > 0$)

## Sandwich Theorem

If $a_n \le b_n \le c_n$ for all $n$ sufficiently large, and $\lim_{n \to \infty} a_n = \lim_{n \to \infty} c_n = L$, then $\lim_{n \to \infty} b_n = L$.

## Properties of Real Numbers and Sequences

### Completeness Axiom

* Every non-empty set of real numbers that has an upper bound also has a least upper bound in the real line.
* **Least Upper Bound (Supremum):** The smallest of all upper bounds, denoted by sup S.

### Types of Sequences

* **Increasing Sequence:** $a_1 < a_2 < a_3 < … < a_n < …$ (strictly increasing if inequality is strict).
* **Decreasing Sequence:** $a_1 > a_2 > a_3 > … > a_n > …$ (strictly decreasing if inequality is strict).
* **Monotonic Sequence:** A sequence that is either increasing or decreasing.
* **Bounded Sequence:** There exist constants $m$ and $M$ such that $m \le a_n \le M$ for all $n \ge 1$.

### Monotonic Sequence Theorem

* Every bounded, monotonic sequence is convergent.
* If an increasing sequence is bounded above by M, its limit is the least upper bound of the sequence.

### Examples of Sequences

* $\{2n\}_{n=1}^\infty$: $2, 4, 6, …, 2n, …$ (Divergent)
* $\{\frac{n}{n+1}\}_{n=1}^\infty$: $\frac{1}{2}, \frac{2}{3}, \frac{3}{4}, …, \frac{n}{n+1}, …$ (Convergent to 1)
* $\{\frac{(-1)^{n+1}}{3^n}\}_{n=1}^\infty$: $\frac{1}{3}, -\frac{1}{9}, \frac{1}{27}, …, \frac{(-1)^{n+1}}{3^n}, …$ (Convergent to 0)
* $\{(-1)^n\}_{n=1}^\infty$: $-1, 1, -1, 1, …$ (Divergent - oscillation)
* $\{\cos n\}_{n=1}^\infty$: $\cos 1, \cos 2, \cos 3, …$ (Divergent - oscillation)

## Geometric Sequence

* $a, ar, ar^2, …, ar^{n-1}, …$ (with $a \neq 0$)
* $\lim_{n \to \infty} r^n = \begin{cases} 0 & \text{if } -1 < r < 1 \\ 1 & \text{if } r = 1 \\ \text{divergent} & \text{otherwise} \end{cases}$

## Common Limits

* $\lim_{n \to \infty} n^{1/n} = 1$
* $\lim_{n \to \infty} \frac{n!}{n^n} = 0$
* $\lim_{n \to \infty} \frac{a^n}{n!} = 0$ for any constant $a$.
* $\lim_{n \to \infty} (1 + \frac{1}{n})^n = e$ (The base of the natural logarithm)

## Recursive Sequences

* A sequence where terms are defined based on previous terms.
* To find the limit of a convergent recursive sequence, assume the limit is L and take the limit of both sides of the recursive relation.
