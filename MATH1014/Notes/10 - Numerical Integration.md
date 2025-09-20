## Numerical Integration Methods

Here's a breakdown of common numerical integration methods:

| Rule/Method    | Formula                                                                                                                        | Geometric Interpretation                                                        |
|:------------- |:----------------------------------------------------------------------------------------------------------------------------- |:------------------------------------------------------------------------------ |
| Left-endpoint  | $L_n = \frac{b-a}{n} [f(x_0) + f(x_1) + f(x_2) + \cdots + f(x_{n-1})]$                                                         | Sum of rectangular areas using the left endpoint of each subinterval.           |
| Right-endpoint | $R_n = \frac{b-a}{n} [f(x_1) + f(x_2) + f(x_3) + \cdots + f(x_n)]$                                                             | Sum of rectangular areas using the right endpoint of each subinterval.          |
| Mid-point      | $M_n = \frac{b-a}{n} [f(\frac{x_0+x_1}{2}) + f(\frac{x_1+x_2}{2}) + f(\frac{x_2+x_3}{2}) + \cdots + f(\frac{x_{n-1}+x_n}{2})]$ | Sum of rectangular areas using the midpoint of each subinterval.                |
| Trapezoidal    | $T_n = \frac{b-a}{2n} [f(x_0) + 2f(x_1) + 2f(x_2) + \cdots + 2f(x_{n-1}) + f(x_n)]$                                            | Sum of trapezoidal areas. Note that $T_n = \frac{L_n + R_n}{2}$.                |
| Simpson's      | $S_{2n} = \frac{b-a}{6n} [f(x_0) + 4f(x_1) + 2f(x_2) + 4f(x_3) + \cdots + 2f(x_{2n-2}) + 4f(x_{2n-1}) + f(x_{2n})]$            | Sum of areas under quadratic curves. Requires an *even* number of subintervals. |

| Rule/Method    | Underestimate             | Overestimate                | Exact                                 |
|:------------- |:------------------------ |:-------------------------- |:------------------------------------ |
| Left-endpoint  | *f(x)* increasing         | *f(x)* decreasing           | *f(x)* constant                       |
| Right-endpoint | *f(x)* decreasing         | *f(x)* increasing           | *f(x)* constant                       |
| Mid-point      | *f''(x) > 0* (concave up) | *f''(x) < 0* (concave down) |                                       |
| Trapezoidal    | *f(x)* concave down       | *f(x)* concave up           | *f(x)* linear                         |
| Simpson's      | *f<sup>(4)</sup>(x) > 0*  | *f<sup>(4)</sup>(x) < 0*    | *f(x)* polynomial of degree 3 or less |

## Simpson's Rule

Simpson's rule leverages the following formula for the integral of a quadratic function $p(x)$ over an interval of width $2h$:

$$\int_{a}^{a+2h} p(x) dx = \frac{h}{3} [p(a) + 4p(a+h) + p(a+2h)]$$

Simpson's rule applies this formula repeatedly on subintervals $[x_0, x_2], [x_2, x_4], \ldots, [x_{2n-2}, x_{2n}]$.

## Error Estimation

To quantify the accuracy of these methods, we define the error as:

$$E = \int_{a}^{b} f(x) dx - \text{Numerical Approximation}$$

Specifically:

$$
\begin{aligned}
&E_{L_n} = \int_{a}^{b} f(x) dx - L_n, \quad E_{R_n} = \int_{a}^{b} f(x) dx - R_n \\
&E_{M_n} = \int_{a}^{b} f(x) dx - M_n, \quad E_{T_n} = \int_{a}^{b} f(x) dx - T_n, \quad E_{S_{2n}} = \int_{a}^{b} f(x) dx - S_{2n}
\end{aligned}
$$

We can use error bounds to estimate the maximum possible error:

* **Trapezoidal Rule:** $|E_{T_n}| \leq \frac{K(b-a)^3}{12n^2}$, where $K \geq |f''(x)|$ for all $a \leq x \leq b$.
* **Midpoint Rule:** $|E_{M_n}| \leq \frac{K(b-a)^3}{24n^2}$, where $K \geq |f''(x)|$ for all $a \leq x \leq b$.
* **Simpson's Rule:** $|E_{S_{2n}}| \leq \frac{K(b-a)^5}{180n^4}$, where $K \geq |f''''(x)|$ for all $a \leq x \leq b$.

$$
\frac{\frac{8}{4}}{3} \cdot (2 + 4 \cdot 1 + 2 \cdot 2 + 4 \cdot 1 + 1) = 10$$
