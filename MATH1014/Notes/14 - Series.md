## Infinite Series

- **Infinite Series:** An infinite series is the sum of a sequence of real numbers.

$$\sum_{n=1}^{\infty} a_n = a_1 + a_2 + … + a_n + …$$  
- **Partial Sum Sequence ($s_n$):** The sequence of partial sums is formed by adding the first $n$ terms of the infinite series.
	- $s_1 = a_1$
	- $s_2 = a_1 + a_2$
	- $s_n = a_1 + a_2 + … + a_n = \sum_{k=1}^{n} a_k$

## Convergence and Divergence

- **Convergent Series:** An infinite series is **convergent** if the limit of its partial sum sequence exists as a finite number.
	- If $\lim_{n \to \infty} s_n = L$, where $L$ is a finite number, the series converges to $L$.
- **Divergent Series:** An infinite series is **divergent** if the limit of its partial sum sequence does not exist as a finite number.
	- This can happen if $\lim_{n \to \infty} s_n = \infty$, $\lim_{n \to \infty} s_n = -\infty$, or if the limit oscillates (does not approach a single value).

## Series with Non-Negative Terms ($a_n \ge 0$ for All $n \ge 1$)

For a series with only non-negative terms, the partial sum sequence $s_n = a_1 + a_2 + … + a_n$ is **non-decreasing** (since we are always adding a non-negative number).

Monotone Convergence Theorem, a non-decreasing sequence either:

- Has **no upper bound**, in which case $\lim_{n \to \infty} s_n = \infty$ (divergent).
- Has **an** upper bound, in which case $\lim_{n \to \infty} s_n$ exists as a finite number (==convergent==).

## Basic Properties of Convergent Series

If $\sum_{n=1}^{\infty} a_n$ and $\sum_{n=1}^{\infty} b_n$ are convergent series, then:

### Sum or Difference

$$\sum_{n=1}^{\infty} (a_n + b_n) = \sum_{n=1}^{\infty} a_n + \sum_{n=1}^{\infty} b_n$$

The sum of two convergent series is convergent, and its sum is the sum of the individual sums.

### Constant Multiple

$$\sum_{n=1}^{\infty} c a_n = c \sum_{n=1}^{\infty} a_n$$

For any constant $c$.

Multiplying a convergent series by a constant results in a convergent series, and its sum is the constant times the original sum.

### Limit Laws Applied to the Partial Sum Sequences

For example, for property "Sum or Difference":

- The partial sum of $\sum (a_n + b_n)$ is $S_n = \sum_{k=1}^{n} (a_k + b_k) = \sum_{k=1}^{n} a_k + \sum_{k=1}^{n} b_k$.
- Taking the limit as $n \to \infty$:

$$\lim_{n \to \infty} S_n = \lim_{n \to \infty} (\sum_{k=1}^{n} a_k + \sum_{k=1}^{n} b_k) = \lim_{n \to \infty} \sum_{k=1}^{n} a_k + \lim_{n \to \infty} \sum_{k=1}^{n} b_k = \sum_{n=1}^{\infty} a_n + \sum_{n=1}^{\infty} b_n$$

### Divergent Series

- **$\sum_{n=1}^{\infty} 1 = 1 + 1 + 1 + …$
- $\sum_{n=1}^{\infty} (-1)^{n+1} = 1 - 1 + 1 - 1 + 1 - 1 + …$  

Since the limit does not exist, the series is **divergent**.

## Geometric Series

> A geometric series is an infinite series of the form $\sum_{n=1}^{\infty} ar^{n-1} = a + ar + ar^2 + … + ar^{n-1} + …$

### Partial Sum of a Geometric Series (for $r \neq 1$)

The $n$-th partial sum is given by the formula:

- $s_n = a(1 + r + … + r^{n-1})$
- Using the factorization $r^n - 1 = (r - 1)(r^{n-1} + r^{n-2} + … + r + 1)$, we can write: $$s_n = a \frac{r^n - 1}{r - 1} = a \frac{1 - r^n}{1 - r}$$

### Convergence of a Geometric Series (for $a \neq 0$)

The convergence of a geometric series depends on the common ratio $r$.

- The sum of the series is: $$\lim_{n \to \infty} s_n = \lim_{n \to \infty} a \frac{1 - r^n}{1 - r} = \frac{a}{1 - r} \lim_{n \to \infty} (1 - r^n) = \frac{a}{1 - r} (1 - \lim_{n \to \infty} r^n)$$
- We need to evaluate $\lim_{n \to \infty} r^n$:
	- The geometric series $\sum_{n=1}^{\infty} ar^{n-1}$ **converges** if **$|r| < 1$** (i.e., $-1 < r < 1$).
	- If it converges, the sum is: $$\frac{a}{1 - r}$$
	- The geometric series **diverges** if **$|r| \ge 1$**.

## Techniques Using Partial Sums (Telescoping Series)

> **Example**: $$\sum_{n=1}^{\infty} \frac{1}{n(n+1)}$$

- We can use partial fraction decomposition: $\frac{1}{n(n+1)} = \frac{1}{n} - \frac{1}{n+1}$.  
- The partial sum is:
	- $s_n = \sum_{k=1}^{n} \frac{1}{k(k+1)} = \sum_{k=1}^{n} (\frac{1}{k} - \frac{1}{k+1})$
	- $s_n = (\frac{1}{1} - \frac{1}{2}) + (\frac{1}{2} - \frac{1}{3}) + (\frac{1}{3} - \frac{1}{4}) + … + (\frac{1}{n} - \frac{1}{n+1})$
	- Most terms cancel out, leaving: $s_n = 1 - \frac{1}{n+1}$.
- The limit of the partial sums is: $\lim_{n \to \infty} s_n = \lim_{n \to \infty} (1 - \frac{1}{n+1}) = 1 - 0 = 1$.
- Since the limit is finite (1), the series is **convergent** and its sum is 1.

## The p-Series

> A p-series is an infinite series of the form $$\sum_{n=1}^{\infty} \frac{1}{n^p} = \frac{1}{1^p} + \frac{1}{2^p} + \frac{1}{3^p} + …$$  
> Where $p$ is a real number.

- **If $p \ge 2$:** The series is **convergent**.
	- For any $n > 1$, $\frac{1}{n^p} \le \frac{1}{n^2}$.
	- The partial sum sequence $s_n = \sum_{k=1}^{n} \frac{1}{k^p}$ is increasing (since terms are positive).
- **If $p \le 1$:** The series is **divergent**.
	- For any $k \ge 1$, if $p \le 1$, then $k^p \le k$. Therefore, $\frac{1}{k^p} \ge \frac{1}{k}$.
	- The partial sum sequence $s_n = \sum_{k=1}^{n} \frac{1}{k^p}$ is increasing.  
	- We can compare the partial sums to the ==harmonic series== $\sum_{k=1}^{\infty} \frac{1}{k}$, which is known to be divergent (its partial sums grow without bound, $\lim_{n \to \infty} \sum_{k=1}^{n} \frac{1}{k} = \infty$).
	- $s_n = \sum_{k=1}^{n} \frac{1}{k^p} \ge \sum_{k=1}^{n} \frac{1}{k}$.
	- Since the partial sums of $\sum \frac{1}{k}$ go to infinity, the partial sums of $\sum \frac{1}{k^p}$ for $p \le 1$ must also go to infinity.

The convergence of the p-series when $1 < p < 2$: **Integral Test**

## Other Common Series with Convergence and Divergence

| Series                                                           | Divergent Condition | Convergent Condition |
| ---------------------------------------------------------------- | ------------------- | -------------------- |
| Harmonic Series<br>$\sum_{n=1}^{\infty} \frac{1}{n}$             | Yes                 | ---                  |
| p-Series<br>$\sum_{n=1}^{\infty} \frac{1}{n^p}$                  | $p \leq 1$          | $p > 1$              |
| Alternating Series<br>$\sum_{n=1}^{\infty} \frac{(-1)^{n+1}}{n}$ | ---                 | Yes                  |
| Geometric Series<br>$\sum_{n=0}^{\infty} ar^n$                   | $\|r\|\geq1$        | $\|r\|<1$            |
| Exponential Series<br>$\sum_{n=0}^{\infty} \frac{x^n}{n!}$       | ---                 | For all $x$          |
