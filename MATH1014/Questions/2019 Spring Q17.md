Let $I = \int_0^1 x^3 \tan^{-1} x \, dx$, and recall that $\frac{d \tan^{-1} x}{dx} = \frac{1}{1+x^2}$.  

## Part A

By applying integration by parts, find a constant $k$ such that:

$$ \int x^3 \tan^{-1} x \, dx = k \left(x^4 \tan^{-1} x - \frac{1}{3} x^3 + x \right) - k \int \frac{1}{1+x^2} \, dx $$  
---

$$
\begin{align}
\int x^3 \tan^{-1} x \, dx  & = \frac{1}{4} \int \tan^{-1} x \, d (x^4) \\
 & = \frac{1}{4} [x^4 \tan^{-1} x] - \frac{1}{4} \int \frac{x^4}{1 + x^2} \ dx \\
 & = \frac{1}{4} [x^4 \tan^{-1} x] - \frac{1}{4} \int \frac{x^4 - 1 + 1}{1 + x^2} \ dx \\
 & = \frac{1}{4} [x^4 \tan^{-1} x] - \frac{1}{4} \int \frac{(x^2 + 1)(x^2 - 1)}{1 + x^2} \ dx - \frac{1}{4} \int \frac{1}{1 + x^2} \ dx \\
& = \frac{1}{4} [x^4 \tan^{-1} x] - \frac{1}{4} \left[ \frac{x^3}{3} - x \right] - \frac{1}{4} \int \frac{1}{1 + x^2} \ dx \\
& = \frac{1}{4} \left[ x^4 \tan^{-1} x - \frac{x^3}{3} + x \right] - \frac{1}{4} \int \frac{1}{1 + x^2} \ dx \\
k  & = \frac{1}{4}
\end{align}
$$

## Part B

Using part (a), or otherwise, find the value of $I = \int_0^1 x^3 \tan^{-1} x \, dx$.  

---

$$
\begin{align}
\int_0^1 x^3 \tan^{-1} x \, dx  & = \frac{1}{4} \left[ x^4 \tan^{-1} x - \frac{x^3}{3} + x \right]^1_{0} - \frac{1}{4} \int^1_{0} \frac{1}{1 + x^2} \ dx \\
 & = \frac{1}{4} \left( \frac{\pi}{4} - \frac{1}{3} + 1 \right) - \frac{1}{4} [ \arctan(x) ]^1_{0} \\
 & = \frac{\pi}{8} - \frac{1}{12} + \frac{1}{4} - \frac{\pi}{8} \\
 & = \frac{3}{12} - \frac{1}{12} = \frac{1}{6}
\end{align}
$$
