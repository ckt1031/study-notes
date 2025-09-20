- We know that for any $n \ge 0$ and $\alpha > 0$, the integral $\int^\infty_0 x^n e^{-\alpha x} dx$ converges.

## Positive Terms: $a_{n} > 0$

### Comparison Test

> Compare your series to a known convergent or divergent series.

Suppose $0 \le a_n \le b_n$ for all $n \ge 1$ (or for $n \ge k$ for some positive integer $k$).

- If $\sum b_n$ is convergent, then $\sum a_n$ is also **convergent**.
- If $\sum a_n$ is divergent, then $\sum b_n$ is also **divergent**.

### Limit Comparison Test

> Compare the behavior of your series' terms to a known series' terms as $n$ approaches infinity.

Suppose $a_n > 0$ and $b_n > 0$, and: $$\lim_{n \to \infty} \frac{a_n}{b_n} = L$$
- If $0 < L < \infty$, then **either both series are convergent or both are divergent**.
- If $L = 0$ and $\sum b_n$ is convergent, then $\sum a_n$ is also **convergent**.
- If $L = \infty$ and $\sum b_n$ is divergent, then $\sum a_n$ is also **divergent**.

## Alternating Series

> $\sum (-1)^{n+1} a_n$ or $\sum (-1)^n a_n$, where $a_n > 0$  
> Checks for convergence of an alternating series based on the behavior of the absolute values of the terms.

The series is convergent if:

- $a_{n+1} \le a_n$ for all $n$ (i.e., the **sequence $a_n$ is decreasing**).
- $\lim_{n \to \infty} a_n = 0$

Example: $\sum_{n=1}^{\infty} \frac{(-1)^{n+1}}{n^p}$, where $p > 0$, is convergent by the Alternating Series Test because $\frac{1}{n^p}$ is a decreasing sequence and $\lim_{n \to \infty} \frac{1}{n^p} = 0$.

## Absolute and Conditional Convergence

### Absolute Convergence

- An infinite series $\sum a_n$ is said to be **absolutely convergent** if the series of absolute values, $\sum |a_n|$, is convergent.
- **Note:** For series with only positive terms ($a_n > 0$), there is no difference between absolute convergence and convergence.
- $\sum_{n=1}^{\infty} \frac{(-1)^{n+1}}{n^2}$ is **absolutely convergent** because $\sum_{n=1}^{\infty} |\frac{(-1)^{n+1}}{n^2}| = \sum_{n=1}^{\infty} \frac{1}{n^2}$, which is a convergent p-series ($p=2 > 1$).

### Conditional Convergence

- If a series $\sum a_n$ is convergent, but the series of absolute values, $\sum |a_n|$, is divergent, then the series $\sum a_n$ is said to be **conditionally convergent**.
- $\sum_{n=1}^{\infty} \frac{(-1)^{n+1}}{n}$ is **conditionally convergent** because the series itself is convergent by the Alternating Series Test, but $\sum_{n=1}^{\infty} |\frac{(-1)^{n+1}}{n}| = \sum_{n=1}^{\infty} \frac{1}{n}$, which is the divergent harmonic series (a p-series with $p=1$).

## Absolute Convergence Tests

### Ratio Test

For a series $\sum a_n$, consider the limit $L = \lim_{n \to \infty} |\frac{a_{n+1}}{a_n}|$.

- If $L < 1$, then the series $\sum a_n$ is **absolutely convergent**.
- If $L > 1$ (including the case $L = \infty$), then the series $\sum a_n$ is **divergent**.
- If $L = 1$, then the Ratio Test is **inconclusive**.

### Root Test

For a series $\sum a_n$, consider the limit $L = \lim_{n \to \infty} \sqrt[n]{|a_n|}$.

- If $L < 1$, then the series $\sum a_n$ is **absolutely convergent**.
- If $L > 1$ (including the case $L = \infty$), then the series $\sum a_n$ is **divergent**.
- If $L = 1$, then the Root Test is **inconclusive**.

## Divergence Test and Integral Test (General Series)

### Divergence Test

If $\lim_{n \to \infty} a_n \neq 0$, the series $\sum a_n$ **must be divergent**.

The converse is not true. If $\lim_{n \to \infty} a_n = 0$, the series **may or may not be convergent**. You need to use other tests.

#### Counterexample for Divergence Test

1. Consider the series $\sum_{n=1}^{\infty} \frac{(-1)^{n}}{n}$, which converges (by the Alternating Series Test), even though $\lim_{n \to \infty} a_n = 0$.
2. Consider harmonic series $\sum_{n=1}^{\infty} \frac{1}{n}$, which diverges, even though $\lim_{n \to \infty} a_n = 0$.

### Integral Test

Suppose $f$ is a continuous, positive, decreasing function on $[1, \infty)$ such that $f(n) = a_n$ for all $n \ge 1$.

The infinite series $\sum_{n=1}^{\infty} f(n)$ is **convergent if and only if** the improper integral $\int_1^{\infty} f(x) dx$ is **convergent**.
