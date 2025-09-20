A curve in the $xy$-plane is defined by the polar equation

$$r = \sin^{2} \theta + 2\sin \theta$$

How many horizontal tangent line does the curve have?

---

$$\frac{dy}{dx} = \frac{r'(\theta) \sin \theta + r(\theta) \cos \theta}{r'(\theta) \cos \theta - r(\theta) \sin \theta}$$

---

$$
\begin{align}
\frac{dr}{d\theta}  & = 2 \sin \theta \cos \theta + 2 \cos \theta \\
 & = 2 \sin 2\theta + 2\cos \theta \\
\frac{dy}{dx}  & = \frac{(2 \sin 2\theta + 2\cos \theta) \sin \theta + (\sin^{2} \theta + 2\sin \theta) \cos \theta}{(2 \sin 2\theta + 2\cos \theta) \cos \theta - (\sin^{2} \theta + 2\sin \theta) \sin \theta} = 0 \\
\sin \theta  & \, \text{or} \cos \theta = 0 \\
\theta  & = 0, \frac{\pi}{2}, \pi, \frac{3}{2} \pi, 2 \pi \\
r(0) = r(\pi) & = r(2\pi)= 0 \\
r \left( \frac{\pi}{2} \right)  & = 3 \\
r \left(  \frac{2\pi}{3} \right)  & = 1 -2 = -1
\end{align}
$$

So we have 3 horizontal tangent.
