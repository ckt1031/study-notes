- North to South (outside)
- South to North (Inside the magnet)  

A magnetic field, denoted by the vector $B$, is defined by the force it exerts on **a moving charged particle**. This magnetic force ==is distinct from the electric force and has unique properties==.

$$
\Phi_{B} = \vec{B} \cdot \vec{A}
$$

![](https://upload.wikimedia.org/wikipedia/commons/9/9a/RightHandOutline.png)

## Conditions for Magnetic Force

1. The particle must be electrically charged, with charge _q_.
2. The particle must be moving, with velocity $v$.

## B-Field

The unit of $B$ is $\mathrm{T}$ or smaller unit $\mathrm{G}$. $1 \ \mathrm{T} = 10^4 \ \mathrm{G}$.

Earth magnetic field is approximately $1 \ \mathrm{G}$

Magnetic force: Only if a charge is moving, there will no effect on the change if the movement is parallel to the B-field

$$
\begin{align}
F  & = |q| v_{\perp} B \\
 & = qvB \sin \phi \\
\vec{F}  & = q \vec{v} \times \vec{B}
\end{align}
$$

![image](https://obsidian-img-studies.tsun1031.xyz/2025/07/12/becdcfa6fa7f424a3a2fff4a613f9ab4.png)

## Magnetic Field Lines

Similar to electric fields, magnetic fields can be visualized using **magnetic field lines**.

- The tangent to a field line at any point gives the direction of the magnetic field B at that point.
- The density of the lines represents the strength of the field.
- Unlike electric field lines that start and end on charges, magnetic field lines always form **closed loops**. This is because magnetic poles always come in pairs (North and South). There is no experimental evidence of isolated magnetic poles, or **magnetic monopoles**.  

Breaking a bar magnet in two results in two new magnets, each with its own N and S pole.

## Gauss's Law for B-Field

SI unit is $\mathrm{Wb \ (weber)}$, $\mathrm{1 wb = 1 T \cdot m^2}$

Some bended B-field (close loops) might eventually bends back to the left hand side for example.

Magnetic field lines are continuous loops with no beginning or end, the total magnetic flux through any closed surface is always zero.

===This law is a fundamental statement that magnetic monopoles do not exist.===

$$
\Phi_{B} = \oint \vec{B} \ d \vec{A} = 0
$$

We cannot break a magnetic into either only north or south, it will be a two single magnetic with north and south pole together.

## Lorentz Force and Work

The magnetic force **never does work** on a moving charged particle.

- The particle's **speed and kinetic energy remain constant**, only its direction of motion changes without electric field.
- **Cannot define a scalar potential energy** (U) for the magnetic force on a single charge, unlike with the electric force.

$$
W_B = \int \vec{F} \ d \vec{l} = 0
$$

## Uniform Circular Motion

> Under uniform B-Field

The magnetic force is always pointing to the center.

> From _PHYS1112_: $$w=\frac{v}{R}$$

$$
\begin{align}
F = ma = |q| vB  & = \frac{mv^2}{R} \\
R  & = \frac{mv}{|q| B}
\end{align}
$$

> Separating protons and electrons with different mass-charge ratio, as proton has greater mass compared to electron and same number of charge.

## Cyclotron Accelerator

How to control the frequency?

$$
T = \frac{2\pi R}{v} = \frac{2\pi}{v} \frac{mv}{|q|B} = 2 \frac{\pi m}{|q| B} = \text{Constant}
$$

The period is constant and independent on the radius of the charge in the accelerator. So we can set the AC current with frequency with $f = T^{-1}$.

Angular frequency (or cyclotron frequency):

$$
w = \frac{|q|B}{m}
$$

Each kinetic increase for ONE pass is $q V_{0}$

## Helical Motion

If the particle's velocity is not perpendicular to the field, its motion is a **helix**.

![](https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcQaF5yOO5LwsfhuxilCOR1_pUIiPc1OFsabkQ&s)

The velocity vector can be broken into two components:

- $v_{\parallel}$: The component parallel to $B$, which **remains constant**.
- $v_{\perp}$: The component perpendicular to $B$, which results in a circular motion.

### A Bubble Chamber

Two particles emerge from the same point. One curves in a tight spiral, the other in a wider spiral.

We know that radius of curvature is proportional to the particle's momentum.

1. The particles curve in opposite directions, indicating they have opposite charges.
2. A particle with a larger radius of curvature has _a higher momentum_ (it's "stiffer" and harder for the field to bend). $p = |q| BR = mv$
3. The paths are spirals of decreasing radius because **the particles lose energy** (and therefore speed/momentum) as they travel through the liquid hydrogen in the chamber, causing their paths to curve more sharply.
