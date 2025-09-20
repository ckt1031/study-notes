Let $f(x) = \frac{\ln (1+e^{2x})}{e^{2x}}$, where $0 \leq 0 < \infty$

If the area under the graph $f$ is rotated about the y-axis to generate a solid of revolution is the volume of the solid finite?

---

> We know that for any $n \ge 0$ and $\alpha > 0$, the integral $\int^\infty_0 x^n e^{-\alpha x} dx$ converges.

$$
\frac{x}{e^x} \frac{\ln (1+e^{2x})}{e^{x}} \lt \frac{x}{e^x}
$$

$$
\ln (1 + e^{2x}) < e^x
$$

When $x$ tends to 0, $\ln (1 + e^{2x}) \to 0$ and $e^x \to 1$  
When $x$ tends to $\infty$, $\ln (1 + e^{2x}) \approx 2x$, but we know that the exponential function grows faster than the polynomial function, so $\ln (1 + e^{2x}) < e^x$.

$$
\begin{align}
V  & = \int_{0}^{\infty} \, 2 \pi x \frac{\ln (1+e^{2x})}{e^{2x}} \ dx  \\
& = 2 \pi \int_{0}^{\infty} \, \frac{x}{e^x} \frac{\ln (1+e^{2x})}{e^{x}} \ dx \\
 \int_{0}^{\infty} \, \frac{x}{e^x}  \ dx  & =  - \int_{0}^{\infty} \, x  \ d (e^{-x}) \\
 & = - [x e^{-x}]_{0}^{\infty} + \int_{0}^{\infty} e^{-x} \, dx  \\
 & =  [-e^{-x} - x e^{-x}]_{0}^{\infty} \\
\lim_{ x \to \infty } \frac{-1}{e^x} - \frac{x}{e^x}  & = 0 \\
  [-e^{-x} - x e^{-x}]_{0}^{\infty}  & = 0 - (-1) = 1
\end{align}
$$

- Since $\int_{0}^{\infty} \, \frac{x}{e^x}  \ dx  = 1$, so $\pi \int_{0}^{\infty} \, 2 \pi x \frac{\ln (1+e^{2x})}{e^{2x}} \ dx$ is finite.
