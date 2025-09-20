A thin disk with a circular hole at its center, called an annulus, has inner radius $R_1$ and outer radius $R_2$. The disk has a uniform positive surface charge density $\sigma$ on its surface.

## Part A

Determine the total electric charge on the annulus.

$$
\begin{align}
Q  & = \pi \sigma (R_{1}^2 -R_{2}^2)
\end{align}
$$

## Part B

The annulus lies in the _yz_-plane, with its center at the origin. For an arbitrary point on the _x_-axis (the axis of the annulus), find the magnitude of the electric field $\vec{E}$. Consider points above the annulus in the figure.

---

$$
\begin{align}
E & = \frac{\sigma x}{4 \epsilon_{0}} \int^{R_{2}}_{R_{1}} \frac{2r}{(x^2 + r^2)^{3/2}} dr \\
 & = - \frac{\sigma x}{2 \epsilon_{0}} \left[ \frac{1}{\sqrt{ x^2+r^2 }} \right]^{R_{2}}_{R_{1}} \\
 & = \frac{\sigma x}{2 \epsilon_{0}} \left[ \frac{1}{\sqrt{ x^2+R_{1}^2 }} - \frac{1}{\sqrt{ x^2+R_{2}^2 }}  \right]
\end{align}
$$

## Part D

A point particle with mass $m$ and negative charge $-q$ is free to move along the $x$-axis (but cannot move off the axis). The particle is originally placed at rest at $x = 0.01 R_1$ and released. Find the frequency of oscillation of the particle.

---

The movement is downwards, acceleration is negative.

$$
\begin{align}
E(x) &  = \frac{-2\sigma x}{4 \epsilon_{0}} \left[ \frac{1}{\sqrt{ x^2 + R_{2}^2 }} - \frac{1}{\sqrt{ x^2 + R_{1}^2 }} \right]  \\
&  = \frac{\sigma x}{2 \epsilon_{0}} \left[ \frac{1}{\sqrt{ x^2 + R_{1}^2 }} - \frac{1}{\sqrt{ x^2 + R_{2}^2 }} \right] \\
F  & = (-q) \cdot E = -kx \\
k  & = \frac{qE}{x}  \\
 & = \frac{q\sigma }{2 \epsilon_{0}} \left[ \frac{1}{\sqrt{ (0.01R_{1})^2 + R_{1}^2 }} - \frac{1}{\sqrt{ (0.01R_{1})^2 + R_{2}^2 }} \right] \\
w  & = \sqrt{ \frac{k}{m} } \\
f  & = \frac{w}{2\pi} \\
 & = \frac{1}{2\pi} \sqrt{ \frac{1}{m} \cdot \frac{q\sigma }{2 \epsilon_{0}} \left[ \frac{1}{\sqrt{ (0.01R_{1})^2 + R_{1}^2 }} - \frac{1}{\sqrt{ (0.01R_{1})^2 + R_{2}^2 }} \right] }
\end{align}
$$
