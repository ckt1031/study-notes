| Situation (Solenoid)                                   | Force      |
| ------------------------------------------------------ | ---------- |
| Magnetic force between adjacent turns                  | Attractive |
| Electric force between adjacent turns?                 | Zero       |
| Magnetic force between opposite sides of the same turn | Repulsive  |

## Magnetic Field of a Moving Charge

A single point charge moving through space generates a magnetic field. Just like a stationary charge creates an electric field, *a moving charge creates a magnetic field in the space around it.*

The direction of $\mathbf{B}$ is perpendicular to the plane containing both the velocity vector $\mathbf{v}$ and the position vector $\mathbf{r}$. This direction is determined by the right-hand rule applied to the cross product.

==The field is zero along the line.==

$$
\mathbf{B} = \frac{\mu_{0}}{4 \pi} \frac{q\mathbf{v} \times \hat{r}}{r^2} = \frac{\mu_{0}}{4 \pi} \frac{q\mathbf{v} \times \vec{r}}{r^3}
$$

> $\hat{r}$ helps define the plane, and $\sin \phi$ helps calculate the strength of the magnetic field that points out of that plane.

**Magnitude of the Field:**

$\phi$ is the angle *between* the velocity vector $\mathbf{v}$ and the position vector $\mathbf{r}$.

$$
B = \frac{\mu_{0}}{4 \pi} \frac{|q|v}{r^2} \sin \phi
$$

**Vacuum permeability**:

$$
\mu_{0} = 4 \pi \times 10^{-7} \ \mathrm{T \cdot m / A}
$$

## The Biot-Savart Law: Magnetic Field of a Current

Describes the magnetic field created by **a small segment of a wire carrying a current**. It is a ==fundamental law==, much like Coulomb's Law in electrostatics.  

$$
d\mathbf{B} = \frac{\mu_{0}}{4 \pi} \frac{I d\mathbf{l} \times \hat{r}}{r^2} = \frac{\mu_{0}}{4 \pi} \frac{I (d\mathbf{l} \times \vec{r})}{r^3}
$$

$$
\mathbf{B} = \frac{\mu_{0}I}{4\pi} \int \frac{d\mathbf{l} \times \hat{r}}{r^2}
$$

> $$I = nqAv_{d} \quad I \ dl= (\frac{q}{\Delta t})v\Delta t = qv$$

## Applications of the Biot-Savart Law

### Magnetic Field of a Long, Straight Conductor

For a straight wire of finite length extending from $y = -a$ to $y = a$, the magnetic field at a point P located a distance x from the wire is found by integration.

$$
\begin{align}
r^2 & = x^2 + y^2 \\
\sin \phi  & = \frac{x}{\sqrt{ x^2 + y^2 }}  \\
dB  & = \frac{\mu_{0} I}{4 \pi} \frac{dl}{r^2} \sin \phi \\
	 & = \frac{\mu_{0} I}{4 \pi} \frac{x dy}{r^2} \frac{x}{\sqrt{ x^2 + y^2 }} \\
 & = \boxed{\frac{\mu_{0} I}{4 \pi x } \frac{2a }{\sqrt{ x^2 + a^2 }}}
\end{align}
$$

**For an Infinitely Long Wire:**

$$
B = \frac{\mu_{0} I}{2 \pi x}
$$

### Force Between Parallel Conductors

- **Parallel currents attract**.
- **Anti-parallel currents repel**.

Two parallel wires carrying currents exert forces on each other.

$$
\begin{align}
B  & = \frac{\mu_{0}I}{2 \pi r} \\
F  & = I^{'} LB \\
\frac{F}{L}  & = \frac{\mu_{0} I I^{'}}{2 \pi r}
\end{align}
$$

## Definition of the Ampere

The SI unit of current, the **ampere (A)**, is formally defined based on the force between two parallel conductors.

One ampere is the constant current which, if **maintained in two straight parallel conductors of infinite length and negligible cross-section**, placed one meter apart in a vacuum, would produce a force between these conductors equal to exactly $2 \times 10^{-7} \ \mathrm{N / m}$

> Why can't $\epsilon_{0}$ (vacuum permittivity) be chosen as an exact value like $\mu_{0}$?

## Magnetic Field of a Circular Current Loop

> Flat coil, not solenoid

For a circular loop of radius $a$ carrying current $I$, the magnetic field can be calculated along the central axis (the x-axis)

- By symmetry, the components of the magnetic field perpendicular to the axis ($dB_{y}$) cancel out.
- For a coil with *N* turns, this value is multiplied by *N*.

$$
\begin{align}
dB_\chi  & = dB \cos\theta \\
B_{x}  & = \frac{\mu_{0}I}{2} \frac{a^2}{(x^2  +a^2)^{3/2}}
\end{align}
$$

### At the Center of the Loop

The field is maximum at the center ($x=0$)

$$
B_{\text{Max}} = \frac{\mu_{0}NI}{2a}
$$

### Magnetic Moment

For distances far from the loop ($x \gg a$), the field expression simplifies to:

> $\mu = NIA$

$$B_{x} \cong \frac{\mu_{0}}{2 \pi} \frac{\mu}{x^3}$$

