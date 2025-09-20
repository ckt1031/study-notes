## What is a Power Series

A power series is an infinite series of the form:

$$
\sum_{n=0}^{\infty} a_{n}(x-a)^{n} = a_{0} + a_{1}(x-a) + a_{2}(x-a)^{2} + \cdots + a_{n}(x-a)^{n} + \cdots
$$

* **$a_n$**: These are constant coefficients.
* **$x$**: This is a variable.
* **$a$**: This is a constant called the **center** of the power series.

## Determining Convergence: Ratio and Root Tests

1. **Ratio Test**
2. **Root Test**

## Possible Convergence Outcomes

### Convergence within an Interval

* **Converges absolutely** for all $x$ such that $|x-a| < R$.  
* **Diverges** for all $x$ such that $|x-a| > R$.
* **Open interval of convergence**, $|x-a| < R$ is equivalent to $a - R < x < a + R$

### Convergence Everywhere

* The series **converges absolutely** for **all real numbers $x$**.
* **Radius of convergence**: $R = \infty$
* The interval of convergence is $(-\infty, \infty)$

### Convergence Only at the Center

* The series **converges only when $x = a$**.
* **Radius of convergence $R = 0$**.
* Interval: $\{a\}$

## Interval of Convergence

* The series *always* converges **absolutely** strictly *inside* the open interval $(a-R, a+R)$.  
* The behavior at the **boundary points $x = a - R$ and $x = a + R$** must be checked **separately**.
* The series may converge or diverge at these points, depending on the specific series.

## Known Functions

Sometimes, a power series is the Taylor series expansion of a known function.

* **Geometric Series:** $\sum_{n=0}^{\infty} x^{n} = \frac{1}{1-x}$ for $|x| < 1$.
* **Exponential Function:** $\sum_{n=0}^{\infty} \frac{x^{n}}{n!} = e^{x}$ for all real $x$. ($R = \infty$).
