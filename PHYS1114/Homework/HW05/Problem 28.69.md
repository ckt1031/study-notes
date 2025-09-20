A long, straight wire with a circular cross section of radius $R$ carries a current $I$. Assume that the current density is not constant across the cross section of the wire, but rather varies as $J = \alpha r$, where $\alpha$ is a constant.

## Part A

By the requirement that $J$ integrated over the cross section of the wire gives the total current $I$, calculate the constant $\alpha$ in terms of $I$ and $R$.

$$
\begin{align}
I  & = \int J \cdot dA \\
 & = \int^R_{0} \alpha r (2 \pi r) \cdot dr \\
\alpha  & = \frac{3I}{2\pi R^3}
\end{align}
$$

## Part B

Use Ampere's law to calculate the magnetic field $B(r)$ for $r \leq R$. Express your answers in terms of $I$.

$$
\begin{align}
I  & = \int^r_{0} J \cdot dA  = \int^r_{0} \alpha r^{'} (2 \pi r^{'} dr) \\
 & = 2 \pi \alpha \left[ \frac{r^3}{3} \right]^r_{0} \\
 & =  \frac{2 \pi \alpha r^3}{3}
\end{align}
$$

$$
\begin{align}
B \cdot (2 \pi r)  & = \mu_{0} \cdot I_{\text{Encl}} \\
B(r)  & = \frac{\mu_{0} \cdot I_{\text{Encl}}}{2 \pi r} \\
B(r)  & = \frac{\mu_{0}}{2 \pi r} \cdot \frac{2 \pi r^3}{3} \cdot \frac{3I}{2\pi R^3} \\
 & = \frac{\mu_{0} I r^2}{2 \pi R^3}
\end{align}
$$

## Part C

Use Ampere's law to calculate the magnetic field $B(r)$ for $r \geq R$. Express your answers in terms of $I$.

> Same as part B.
