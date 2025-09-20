## Average Value of a Continuous Function

$$
\begin{align}
a = x_0 < x_{1}  & < \dots < x_{n} = b \\
\Delta x  & = \frac{b - a}{n}
\end{align}
$$

Let $f$ be a continuous function on the interval $[a, b]$. The average value of $f$ over $[a, b]$, denoted by $f_{\text{ave}}$, is defined as:

$$
f_{\text{ave}} =  \lim_{ n \to \infty } \frac{1}{b-a} \sum^n_{i=1} f(c_{i}) \Delta x = \frac{1}{b-a} \int_{a}^{b} f(x) \, dx
$$

*Explanation:* This formula calculates the average height of the function $f(x)$ over the interval $[a, b]$. It's the integral of the function (area under the curve) divided by the length of the interval.

*Example:* Consider $f(x) = x^2$ on the interval $[0, 2]$. Then  
$$ f_{\text{ave}} = \frac{1}{2-0} \int_0^2 x^2 dx = \frac{1}{2} \left[\frac{x^3}{3} \right]_0^2 = \frac{1}{2} \cdot \frac{8}{3} = \frac{4}{3} $$

## Mean Value Theorem for Integrals

If $f$ is continuous on $[a, b]$, then there exists a number $c$ in $[a, b]$ such that:

$$
\int_{a}^{b} f(x) \, dx = f(c)(b-a)
$$

Equivalently,

$$
f(c) = \frac{1}{b-a} \int_{a}^{b} f(x) \, dx = f_{\text{ave}}
$$

*Explanation:* This theorem guarantees that there's at least one point $c$ in the interval $[a, b]$ where the function's value $f(c)$ is equal to the average value of the function over that interval. Geometrically, the area under the curve of $f(x)$ from $a$ to $b$ is equal to the area of a rectangle with base $(b-a)$ and height $f(c)$.

*Tip:* The Mean Value Theorem for Integrals is an existence theorem. It tells you that such a $c$ exists, but it doesn't tell you *how* to find it. To find $c$, you need to compute $f_{\text{ave}}$ and then solve the equation $f(c) = f_{\text{ave}}$ for $c$.

*Example:* Let $f(x) = x$ on the interval $[1, 3]$. Then  
$$ f_{\text{ave}} = \frac{1}{3-1} \int_1^3 x \, dx = \frac{1}{2} \left[\frac{x^2}{2} \right]_1^3 = \frac{1}{2} \left(\frac{9}{2} - \frac{1}{2} \right) = \frac{1}{2} \cdot \frac{8}{2} = 2 $$  
To find $c$, we solve $f(c) = c = 2$. Since $2$ is in the interval $[1, 3]$, the Mean Value Theorem for Integrals is satisfied.
