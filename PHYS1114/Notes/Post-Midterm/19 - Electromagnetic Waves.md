## The Nature of Electromagnetic (EM) Waves

An electromagnetic wave is a ==self-sustaining disturbance of electric and magnetic fields== that propagates through space.

The core concept, derived from Maxwell's Equations, is that a time-varying field of one type generates a field of the other type:

- A **time-varying magnetic field** ($B$) ==creates an electric field== ($E$), as described by Faraday's Law.  
- A **time-varying electric field** ($E$) ==creates a magnetic field== ($B$), as described by the Ampere-Maxwell Law.

This continuous, mutual generation, $E \to B \to E \to \dots$, allows the wave to propagate even **through a vacuum without any charges or medium**. Any accelerating charge is a source of electromagnetic waves.

==Any accelerating charge is a source of electromagnetic waves.==

## Speed of an EM Wave

To understand the properties of an EM wave, we can analyze a simplified "plane wave" moving in the +x direction. In this model, behind the wavefront, the E field is uniform and points in the +y direction, while the B field is uniform and points in the +z direction. Ahead of the wave, both fields are zero.

#missing-draw

### Applying Faraday's Law

We imagine a stationary rectangular loop of height $a$ in the xy-plane, $c \ dt$ is moved distance in a time interval $dt$.

$$
\begin{align}
\oint E \cdot dl  & = - \frac{d\Phi_{B}}{dt} = Ea  \\
Ea  & = -\frac{d}{dt} (-B \ \text{Area}) \\
 E a& = B ac \\
E  & = \boxed{cB}
\end{align}
$$

### Applying Ampere's Law

$$
\begin{align}
\oint B \cdot dl  & = \mu_{0} \epsilon_{0}  \frac{d\Phi_{E}}{dt} \\
Ba  & = \mu_{0} \epsilon_{0} acE \\
B  & = \mu_{0} \epsilon_{0} cE
\end{align}
$$

### Finding Speed of light

$$
\begin{align}
B  & = \mu_{0} \epsilon_{0} c (cB) \\
1  & = \mu_{0} \epsilon_{0} c^2 \\
c  & = \frac{1}{\sqrt{ \mu_{0} \epsilon_{0} }} \approx 3 \times 10^8 \ \mathrm{m/s}
\end{align}
$$

## Sinusoidal EM Waves

- **No Medium Required**: EM waves can travel through a vacuum.
- **Constant Speed in Vacuum**
- **Transverse Nature**: The electric field E and magnetic field B are always perpendicular to each other and to the direction of wave propagation.
- ==In Phase==: In a traveling wave, the E and B fields are always in phase, meaning they reach their maximum and minimum values at the same time and place.
- **Direction of Propagation**: The direction of travel is given by the cross product: $$\vec{P} = E \times B$$

### Wave Equations

A sinusoidal EM wave traveling along the x-axis:

$$
k = \frac{2\pi}{\lambda} \quad c = f \lambda = \frac{\omega}{k} 
$$

**Wave traveling in the +x direction:** (Incident wave)

$$
\begin{align}
E(x, t)  & = \hat{j} E_{\text{max}} \cos (kx - \omega t) \\
B(x, t)  & = \hat{k} B_{\text{max}} \cos (kx - \omega t)
\end{align}
$$

**Wave traveling in the -x direction:** (Reflected wave)

$$
\begin{align}
E(x, t)  & = \hat{j} E_{\text{max}} \cos (kx + \omega t) \\
B(x, t)  & = - \hat{k} B_{\text{max}} \cos (kx + \omega t)
\end{align}
$$

## EM Waves in Matter

When an EM wave travels through a **dielectric material** (like glass or water), ==its speed decreases.==

$$
v = \frac{1}{\sqrt{ \epsilon \mu }}= \frac{1}{\sqrt{ K K_{m} \epsilon_{0} \mu_{0} }} = \frac{c}{\sqrt{ KK_{m} }}
$$

The **refractive index (n)** of the material is the ratio of the speed of light in vacuum to the speed in the material:

$$
n = \frac{c}{v} = \sqrt{ KK_{m} }
$$

## Standing Electromagnetic Waves

> The only way for the tangential electric field to be permanently zero at the walls is if the walls are located at nodal planes of the electric field.

When an EM wave reflects from a perfect conductor, the incident and reflected waves interfere to create a **standing wave**.

At the surface of the conductor, the electric field parallel to the surface ==must always be zero==.

$$
\begin{align}
E_{inc}  &  = E_{max} \cos (kx-\omega t) \\
E_{ref}  & = - E_{max} \cos (kx + \omega t)
\end{align}
$$

### Key Features of Standing Waves

- The $\mathbf{E}$ and $\mathbf{B}$ fields are $90^{\circ}$ ==out of phase==. The electric field is maximum when the magnetic field is zero, and vice-versa.
- The wave has fixed locations of zero amplitude, called **nodes**, and maximum amplitude, called **antinodes**.
- The nodal planes of E correspond to the anti-nodal planes of B.

---

If a second conducting wall is placed at a distance L, a resonant cavity is formed.

==Standing waves can only exist if the length L is an integer multiple of half-wavelengths:==

A standing wave is used in a microwave oven for one main reason: **to concentrate energy for efficient heating**.

$$
L = n \frac{\lambda_{n}}{2}
$$

This is the principle behind a **microwave oven**, which creates a standing wave that is strongly absorbed by water molecules in food.

## Energy Density

$$
u = \frac{1}{2} \mathcal{E}_{0} E^2 + \frac{1}{2 \mu_{0}} B^2
$$

$$
I = uc
$$

## Intensity of EM Wave

**Magnetic field**

$$
I = \frac{1}{2} \frac{v}{\mu} B^2_{\text{max}}
$$

**Both electric and magnetic fields**

$$
I = \frac{E_{\text{max}}B_{\text{max}}}{2 \mu}
$$

**For a wave in a vacuum**

$$
I = \frac{1}{2} \epsilon_{0} cE^2_{\text{max}} \quad \text{or} \quad I= \frac{c}{2\mu_{0}} B^2_{\text{max}}
$$
