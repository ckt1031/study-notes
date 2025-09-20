A very long **insulating** cylinder has radius $R$ and carries positive charge distributed throughout its volume. The charge distribution has cylindrical symmetry but varies with perpendicular distance from the axis of the cylinder. The volume charge density is $\rho(r)=\alpha(1-r/R)$, where $\alpha$ is a constant with units $\mathrm{C}/\mathrm{m}^{3}$ and $r$ is the perpendicular distance from the center line of the cylinder.

![[Drawing 2025-06-25 14.29.14.excalidraw]]

## Part A

Derive an expression for $\mathrm{E}(r)$, the electric field as a function of $r$ for $r < R$.

---

$$
\begin{align}
dQ  & = \rho \cdot dV \\
\int d Q  & = \alpha \int^r_{0} \left( 1-\frac{r}{R} \right)2 \pi r L  \cdot dr \\
 & = 2 \alpha \pi L \int^r_{0} \left( r - \frac{r^2}{R} \right) dr \\
 & = 2 \alpha \pi L \left[ \frac{r^2}{2} - \frac{r^3}{3R} \right] \\
\Phi_{E}  & = E \cdot (2 \pi r L) = \frac{2 \alpha \pi L \left[ \frac{r^2}{2} - \frac{r^3}{3R} \right]}{\epsilon_{0}} \\
E & = \frac{\alpha r}{\epsilon_{0}} \left( \frac{1}{2} - \frac{r}{3R} \right)
\end{align}
$$

## Part B

Derive an expression for $E(r)$, the electric field as a function of $r$ for $r>R$.

---

$$
\begin{align}
Q & = \int \rho \cdot dV = 2 \alpha \pi L \left[ \frac{R^2}{2} - \frac{R^3}{3R} \right]  \\
 & = \int \rho \cdot dV = \alpha \pi L \left[ \frac{R^2}{3} \right] \\
E \cdot (2 \pi r L)  & = \frac{\alpha \pi L \left[ \frac{R^2}{3} \right]}{\epsilon_{0}} \\
E  & = \frac{\alpha R^2}{6 r \epsilon_{0}}
\end{align}
$$

## Part C

Do you agree for $r=R$?

$$
\begin{align}
E_{r < R}  & = \frac{\alpha r}{\epsilon_{0}}\left( \frac{1}{2} - \frac{1}{3} \right) \\
& =  \frac{\alpha r}{6\epsilon_{0}} \\
E_{r > R}  & = \frac{\alpha r}{6 \epsilon_{0}} = E_{r < R}
\end{align}
$$

It's continuous function, so the field is continuous at $r=R$.
