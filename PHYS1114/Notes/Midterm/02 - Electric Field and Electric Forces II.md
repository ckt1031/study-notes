- Infinity Long Distance
- Infinity Large Surface

## Electric Field Lines

1. Start from a **positive charge**.
2. End at a **negative charge** (or extend to infinity).
3. **Repel** each other (they do not cross).
4. **Density of Lines:** A larger density of field lines indicates a stronger electric field. Lines are closer together where the field is strong, farther apart where it is weaker.
5. **Not Trajectories:** Field lines indicate the direction of **acceleration** of a test charge, not its velocity (or trajectory).

## Superposition of Electric Fields (Continuous Charge Distributions)

To calculate the electric field due to a continuous charge distribution, the distribution is divided into **infinitesimal charge elements**, each treated as a point charge. The total field is then found by ==integrating the contributions from all these elements==.

- Divide the charge distribution into infinitesimal elements $dQ$.
- Calculate the electric field $d\vec{E}$ due to each $dQ$ using the point charge formula $$d\vec{E} = \frac{1}{4\pi\epsilon_0} \frac{dQ}{r^2} \hat{r}$$
- Integrate $d\vec{E}$ over the entire charge distribution: $\vec{E} = \int d\vec{E}$. This often involves component-wise integration $$\vec{E} = E_x \hat{i} + E_y \hat{j} + E_z \hat{k}$$

### Uniform Charge Distribution

1. Linear charge: $\mathrm{d} q = \lambda \ \mathrm{d}l$
2. Surface charge: $\mathrm{d} q = \sigma \ \mathrm{d} l$
3. Volume charge: $\mathrm{d} q = \rho \ \mathrm{d} V$

### Field of a Charged line Segment

- **Linear charge density**: $\lambda = \frac{Q}{\text{Length of rod}}$

$$dE = \frac{1}{4\pi\epsilon_0} \frac{\lambda dy}{r^2}$$

- **Infinitely long segment**: $x \ll a$, then the perpendicular distance is only the key for E-field: $$E = \frac{1}{2\pi\epsilon_0} \frac{\lambda}{x}$$

#### Perpendicular Bisector

![[02-middle-line-segment.excalidraw]]

We consider a line segment of length $2a$, centered at the origin and lying along the y-axis (from $y=-a$ to $y=+a$).

For line segment lying over y-axis vertically, y component of $d \vec{E}$ is cancelled out.

For horizontal rod, lying on x-axis, substitute $x$ as the distance between the rod and point in perpendicular distance.

> Can memorize the integration result, this is not a MATH course.

$$
\text{Linear Charge Density} = \lambda = \frac{Q}{2 a}
$$

$$
\begin{align}
\text{Distance from dQ to P}  & = r = \sqrt{ x^2 + y^2}  \\
dQ   & = \lambda dy \\
\cos \alpha  & = \frac{x}{r} = \frac{x}{\sqrt{ x^2 + y^2}} \\
d E_{x}  &  = k_{e} \frac{\lambda dy}{x^2 + y^2} \cdot \frac{x}{\sqrt{ x^2 + y^2}} \\
 & = k_{e} \lambda x \frac{dy}{(x^2 + y^2)^{3/2}}  \\
E_{x}  & = k_{e} \lambda x \int_{-a}^a \frac{dy}{(x^2 + y^2)^{3/2}} \\
 & = k_{e} \lambda x \left[ \frac{1}{x \sqrt{ x^2 + y^2 }} \right]^a_{-a} \\
 & = k_{e} \lambda \frac{2a}{x \sqrt{ x^2 + a^2 }} \\
 & = k_{e} \frac{Q}{x \sqrt{ x^2 + a^2 }}
\end{align}
$$

For infinite long distance, $x \to \infty$, $\sqrt{ x^2 + a^2 } \to \sqrt{ x^2 } = x$  
For infinite long rod, $a \to \infty$, $\frac{x}{a} \to 0$, $\sqrt{ 1 + \left(\frac{x}{a} \right)^2 } \to 1$.

### Field of a Charged Ring

![[02-middle-charged-ring.excalidraw]]

Similar to the ling segment, but length is the circumference.

$$
\text{Linear Charge Density} = \lambda = \frac{Q}{2\pi a}
$$

$$
\begin{align}
s  & = a \ \theta \\
d Q  & = \lambda 2 \pi \ (a d \theta) \\
r  & = \sqrt{ x^2 + a^2 } \\
d E_{x}  &  = k_{e} \frac{\lambda ds}{r^2} \cdot \frac{x}{r} \\
 & = k_{e} \lambda x \frac{ds}{r^3} \\
E_{x}  & = k_{e} \lambda x \frac{1}{r^{3}} \int^a_{-a} ds = k_{e} \lambda x \frac{1}{r^{3}} (2 \pi a) \\
 & = \frac{k_{e} \lambda x}{(x^2 + a^2)^{3/2}} (2 \pi a)
\end{align}
$$

If the point is in the center of ring, $\vec{E} = 0$, _every single pair_ of diametrically opposed charge elements on the entire ring.

### Portion of Ring

### Field of a Uniformly Charged Disk

![[02-charged-disk-ef.excalidraw]]

- $r$ stands for the radius of infinitesimal ring.

$$
\text{Surface Charge Density} = \sigma = \frac{Q}{\pi R^2}
$$

$$
\begin{align}
dQ  & = \sigma (2 \pi r dr)  \\
d E_{x} & = \frac{x k_{e} \sigma 2 r\pi dr }{(x^2+r^2)^{3/2}}  \\
\int \frac{r dr}{(x^2 + r^2)^{3/2}}  & = -\frac{1}{\sqrt{x^2 + r^2}} \\
E_{x}  & = k_{e} 2 \pi x \sigma \int^R_{0} \frac{rdr}{(x^2 + r^2)^{3/2}} \\
 & = k_{e} 2 \pi x \sigma \left[ -\frac{1}{\sqrt{x^2 + r^2}} \right]^R_{0} \\
 & = k_{e} 2 \pi x \sigma \left[ \frac{1}{x} - \frac{1}{\sqrt{ x^2 + R^2 }} \right] \\
 & = \frac{\sigma}{2\epsilon_{0}} \left[ 1 - \frac{x}{\sqrt{ x^2 + R^2 }} \right]
\end{align}
$$

- For infinite long distance: $E = 0$
- For infinite large disk: $$E=\frac{\sigma}{2 \epsilon_{0}}$$

### Electric Field of Infinite Parallel Plates

![[02-inf-parallel-plates.excalidraw]]

The upper parallel plate with charge $- \sigma$ and the lower plate with charge $+ \sigma$, with distance $d$.

- Electric field strength of area **BETWEEN** both plates is $E = \frac{\sigma}{\epsilon_0}$.
- Electric field strength of area **outside** (above the upper plate and below the bottom plate) is $E = 0$

### How to Achieve a Uniform Electric Field?

- **Infinite Extent (or Effectively Infinite)**
- Uniform Surface Charge Density ($\sigma$)
- Perfectly Parallel Plates (Planar)
- Ideal Conductors, the electric field within the conductor itself is zero (In next lecture notes).

## Field of an Electric Dipole

> An electric dipole is a pair of equal and opposite charges, $+q$ and $-q$, separated by a fixed distance $d$.

Electric Dipole Moment ($\vec{p}$): $\vec{d}$ is a vector from the negative charge to the positive charge. $$\vec{p} = q\vec{d}$$

![[02-efield-dipole.excalidraw]]

For $y \gg d$:

$$
\begin{align}
E_{y} & = \frac{q}{4 \pi \epsilon_{0}}  \left[ \frac{1}{\left( y - \frac{d}{2} \right)^2} - \frac{1}{\left( y + \frac{d}{2} \right)^2} \right]   \\
 & = \frac{q}{4 \pi \epsilon _{0}} \frac{y^2 + dy + \left( \frac{d}{2} \right)^2 - y^2 + dy - \left( \frac{d}{2} \right)^2}{\left( y^2 - \left( \frac{d}{2} \right)^2 \right)^2} \\
\text{When}\  y  &  \ll d,  \ \left( y^2 -  \left( \frac{d}{2} \right)^2   \right)^2 \approx y^4 \\
 E_{y}  & = \frac{q}{4 \pi \epsilon_{0}} \frac{2dy}{y^4} \\
 & = \frac{qd}{2 \pi \epsilon_{0} y^3}= \frac{p}{2 \pi \epsilon_{0} y^3}
\end{align}
$$

- The electric field of a dipole decays as $1/y^3$ (or $1/r^3$ in general) **when far away**, which is faster than the $1/r^2$ decay of a single point charge.

## Electric Dipole in a Uniform Electric Field

Net Force: The total force on the dipole is the vector sum of these two forces, which is zero:  
$\mathbf{F}_{+} + \mathbf{F}_{-} = 0$. This means the dipole's center of mass will not accelerate.

Torque: Although the net force is zero, the forces create a torque that causes the dipole to rotate. The torque, $\tau$, is calculated as the sum of the torques produced by each force about the center of the dipole.

$$
\begin{align}
p  & = qd \\
\tau  & = p \times E \\
\tau  & = p E \sin \phi
\end{align}
$$

### Potential Energy of an Electric Dipole

The work $dW$ done by the torque in rotating the dipole through a small angle $d\phi$ is $dW = \tau d\phi = -pE \sin\phi d\phi$. The negative sign indicates that the torque does positive work when the angle $\phi$ decreases.

Work Done:

$$W = -\int_{\phi_1}^{\phi_2} pE \sin\phi \, d\phi = pE \cos\phi_2 - pE \cos\phi_1$$

Potential Energy:

$$
U = - p \cdot E
$$
