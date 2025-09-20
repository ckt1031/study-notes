## What Are Improper Integrals?

Improper integrals extend the concept of definite integrals to:

- **Infinite intervals**: The integration takes place over an interval that extends to infinity (e.g., $[a, \infty)$, $(-\infty, b]$, or $(-\infty, \infty)$).
- **Unbounded functions**: The function being integrated is unbounded at one or more points within the integration interval.
- **Mixtures of both**: Combining infinite intervals and unbounded functions.

## Two Basic Types of Improper Integrals

### Type I: Infinite Intervals

- Integral from a to infinity: Represents the area under the curve from $a$ to $\infty$

$$\int_a^\infty f(x) dx = \lim_{L \to \infty} \int_a^L f(x) dx$$  

- Integral from negative infinity to $b$: Represents the area under the curve from $-\infty$ to $b$

$$\int_{-\infty}^b f(x) dx = \lim_{L \to -\infty} \int_L^b f(x) dx$$

- Integral from negative infinity to infinity: Break the integral into two parts at an arbitrary point $a$, then evaluate each as a Type I integral

$$\int_{-\infty}^\infty f(x) dx = \int_{-\infty}^a f(x) dx + \int_a^\infty f(x) dx$$

### Type II: Unbounded Functions on Finite Intervals

These involve functions that are unbounded at one or more endpoints within a finite interval $[a, b]$.

- Function unbounded at 'b'. The limit is taken as $L$ approaches $b$ from the left side, as the function becomes unbounded as $x$ approaches $b$.

$$\int_a^b f(x) dx = \lim_{L \to b^-} \int_a^L f(x) dx$$  

- Function unbounded at 'a': The limit is taken as $L$ approaches $a$ from the right side, as the function becomes unbounded as $x$ approaches $a$  

$$\int_a^b f(x) dx = \lim_{L \to a^+} \int_L^b f(x) dx$$

- Function unbounded at a point 'c' within the interval $[a, b]$: Break the integral into two parts at the point of unboundedness 'c', then evaluate each as a Type II integral  

$$\int_a^b f(x) dx = \int_a^c f(x) dx + \int_c^b f(x) dx$$

## Convergence and Divergence

- **Convergent:** An improper integral is **convergent** if the corresponding limit ==exists and is a finite value==.
- **Divergent:** An improper integral is **divergent** if the corresponding limit ==does not exist or is infinite==.

## Determining Convergence or Divergence (Beyond Exact Computation)

### Comparison Test

Suppose $f(x)$ and $g(x)$ are non-negative, continuous functions on the interval $[a, b]$ such that $0 \le f(x) \le g(x)$.

1. If $\int_a^\infty g(x) dx$ is convergent, then $\int_a^\infty f(x) dx$ must also be convergent.  
   (If the "larger" integral converges, the "smaller" one must too).
2. If $\int_a^\infty f(x) dx$ is divergent, then $\int_a^\infty g(x) dx$ must also be divergent.  
   (If the "smaller" integral diverges, the "larger" one must too).

> For $f(x) \ge 0$: For non-negative functions, $\int_a^\infty f(x) dx$ will either converge to a finite value or diverge to $\infty$.

## Basic Properties of Improper Integrals

> For continuous functions f, g on $[a, \infty)$

- $\int_a^\infty f(x) dx$ is convergent if and only if $\int_N^\infty f(x) dx$ is convergent for some number $N > a$.  
- $\int_a^\infty (f(x)+g(x)) dx = \int_a^\infty f(x) dx + \int_a^\infty g(x) dx$ whenever the integrals on the right-hand side are convergent.  
- $\int_a^\infty kf(x) dx = k \int_a^\infty f(x) dx$ (where $k$ is a constant), whenever the integral on the right-hand side is convergent.  
- If $\int_a^\infty |f(x)| dx$ is convergent, then $\int_a^\infty f(x) dx$ must also be convergent.
