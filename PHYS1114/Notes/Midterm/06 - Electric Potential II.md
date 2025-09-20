![](https://www.youtube.com/watch?v=4QvsNAnuLUw)

## Potential of Charged Conducting Sphere

A spherical conductor of radius $R$ with total charge $q$ is a canonical example.

- **Outside Sphere**: $r > R$, $\vec{E}$ is radially outwards.

$$
V(r) - V(\infty) = - \int_{\infty}^{r} E\cdot  -\int^{r}_{\infty}\!E\,\operatorname{d}dl =- \int_{\infty}^{r} \frac{1}{4 \pi \epsilon_{0}} \frac{q}{r^{'2}} d r^{'}
$$

$$
V(r) = \frac{1}{4 \pi \epsilon_{0}} \frac{q}{r}
$$

- **Inside the sphere**: $r < R$, since $\vec{E} = 0$ inside the conductor, the **potential difference between any two points inside is zero**.

$$
V(r) - V(R) = 0
$$

$$
V(r) = V(R) = \boxed{\frac{1}{4 \pi \epsilon_{0}} \frac{q}{R}}
$$

---

Assume we have two conducting sphere with $R_{1}$ and $R_{2}$, and $q_{1}$ and $q_{2}$ charge. We connect them with a conducting wire. ==Their voltage will be equalized==, $V_{1} = V_{2}$ since there will be a path way $\int \vec{E} \cdot d \vec{l}$, where $\vec{E} = 0$ in total conductor.

## Oppositely Charged Parallel Plates

![[06-efield-plates-voltage.excalidraw]]

For two large, parallel conducting plates separated by a distance $d$, their E field is uniform.

$$
\begin{align}
\text{Voltage between plates}: V_{a} - V_{b}  & = \int_{a}^{b} E \cdot dl = \boxed{E \cdot d} \\
\text{Voltage between point and plate}: V_{y} - V_{b}  & = \boxed{E\cdot y} = \boxed{\frac{\sigma}{\epsilon_{0}} \cdot y} \quad y \in (0, d]
\end{align}
$$

Let say plate a is upper and plate b is lower, if $V_{a} > V_{b}$, then $E$ is directed downwards. One plate with larger potential is positively charged and the other negatively charged.

**With reference point**: $V(y) = \Delta V + V_{\text{ref}}$

## The Infinite Line of Charge and the Reference Point

$$
\begin{align}
E  (2 \pi r L)  & = \frac{Q}{\epsilon_{0 \frac{Q}{\mathrm{\epsilon_0}}}} = \frac{\lambda L}{\epsilon_{0}} \\
V(r)  & = - \int^r_{\infty} \frac{\lambda}{2 \pi \epsilon_{0} r^{'}} \cdot d r^{'} = \infty
\end{align}
$$

**The voltage is infinite at infinity**, so we need to choose better a reference point.

For a charged cylinder of radius $R$, *a convenient choice* is to set the potential on its surface to zero, $V(R) =0$.

$$
\begin{align}
V(r) - V(R)  & = - \frac{\lambda}{2 \pi \epsilon_{0}} \left[ \ln(r^{'}) \right]^r_{R} \\
V(r) & = \boxed{\frac{\lambda}{2 \pi \epsilon_{0}} \ln \left|\frac{R}{r}\right|} <0
\end{align}
$$

- If $r= R$, $V(r) = 0$
- If $r > R$, $V(r) > 0$
- If $r < R$, $V(r) = 0$, by definition of electrostatic, no e-field inside the conductor rod with radius $R$.

## A Ring of Charge

![[02-middle-charged-ring.excalidraw]]

$$
\begin{align}
V  & = \int \frac{1}{4 \pi \epsilon_{0}} \frac{dq}{r} = \frac{1}{4 \pi \epsilon_{0}} \int^{2\pi}_{0} \frac{\lambda a}{r} \cdot d\phi \\
 & = \frac{Q}{4 \pi \epsilon_{0} r} \\
 & = \boxed{\frac{1}{4 \pi \epsilon_{0}} \frac{Q}{\sqrt{ x^2 + a^2 }}}
\end{align}
$$

## A Finite Line of Charge

![[02-middle-line-segment.excalidraw]]

$$
\begin{align}
V & = \int^a_{-a} \frac{1}{4 \pi \epsilon_{0}} \frac{dq}{r} = \frac{1}{4 \pi \epsilon_{0}} \frac{Q}{2a} \int^a_{-a} \frac{dy}{\sqrt{ x^2+y^2 }} \\
 & = \frac{1}{4 \pi \epsilon_{0}} \frac{Q}{2a} \left[ \ln \left| \sqrt{ x^2 +y^2 } +y\right|\right]^a_{-a} \\
 & = \boxed{\frac{1}{4 \pi \epsilon_{0}} \frac{Q}{2a} \ln \left( \frac{\sqrt{ a^2 +x^2 } + a}{\sqrt{ a^2 +x^2 } -a} \right)}
\end{align}
$$

When $a \to \infty$, $\ln\left(\frac{\sqrt{ a^2 } + a}{\sqrt{ a^2 } - a} \right) =\ln\left(\frac{2a}{0} \right) = \infty$, the voltage is infinity.  
When $x \to \infty$, $\ln (\frac{1}{1}) = 0$

**The reference point assumptions:** The voltage is set zero when the distance is infinity.

## Stronger E-field in Sharp Edges

![[Drawing 2025-06-25 11.24.03.excalidraw]]

Edge of a non-smooth conductor has greater e-field.

$$
\sigma \propto \frac{1}{r} \quad E \propto \sigma
$$

Smaller curvature radius implies a stronger e-field with more charges accumulated on the surface of the edge.

This is why the thunderstorm strikes trees more often

## Equipotential Surfaces and Conductors

![[06-equipotential-surfaces.excalidraw]]

Properties of equipotential surfaces:

1. **No work is done** when a test charge moves along an equipotential surface, the potential difference $\Delta V$ between any two points on an equipotential surface is zero
2. **Perpendicularity to Field Lines**: Since ==no work is done== moving along an equipotential, there can be no component of the electric force.
3. **Direction of Field**: The electric field $\vec{E}$ always points in the direction of the greatest decrease in potential. A positive test charge, if released, will "fall" from high $V$ to low $V$.
4. **Field Strength and Spacing**: Where equipotential surfaces ==are closely packed==, the potential changes quickly, and ==the electric field is strong==. Where they are far apart, the field is weak. This is analogous to a steep hill having closely spaced contour lines.

Conductors as Equipotential Volumes:

> Result: **The potential anywhere on the surfaces, inside the conductor, and inside empty cavities are all the same**

> Proof by contradiction. $\vec{E} = 0$ due to Guass's Law

1. Assume, for contradiction, that the *potential inside a cavity is not uniform*.
2. This would mean there exists a point $P$ inside the cavity with a potential $V_P$ different from the potential of the conductor's inner surface, $V_A$.
3. If this were true, we could construct an *equipotential surface* $B$ through point $P$.
4. An electric field must exist in the region between surface $A$ and surface $B$, pointing from the higher potential surface to the lower potential surface.
5. An electric field passes through this Gaussian surface, there must be a non-zero net electric flux.
6. However, this Gaussian surface is in a region where there are no charges. By Gauss's Law, a non-zero flux implies a non-zero enclosed charge, which is a contradiction.
7. Therefore, the potential must be **constant throughout the empty cavity** and **equal to the potential of the conductor itself**.

P cannot touch the conductor, because they will share the same equipotential surfaces.

## Gradient

$$
dV = - E \cdot dl = - (E_{x} dx + E_{y} dy + E_{z} dz)
$$

Consider a change only in x-direction, we can differentiate with respect to one variable while holding other constant. Differentiate $V(x,y,z)$ as if $y$ and $z$ are constant

$$E_x = -\frac{\partial V}{\partial x}$$

---

Example of partial derivative:

$$
\begin{align}
f(x, y, z)  & = \frac{xy}{xy+zy}\\
\frac{\partial f}{\partial y}  & = 
\end{align}
$$

### Gradient Operator $\nabla$

This is to transform a scalar function to a vector field.

$$
E = - \nabla V = - \left( \frac{\partial V}{\partial x} \hat{i} + \frac{\partial V}{\partial y} \hat{j}+ \frac{\partial V}{\partial z} \hat{k} \right)
$$
