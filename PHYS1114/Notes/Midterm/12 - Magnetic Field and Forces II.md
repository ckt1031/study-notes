When both an electric field $E$ and a magnetic field $B$ are present, the total force on a charged particle is the Lorentz force:

$$\vec{F}=q\vec{E} +q\vec{v} \times \vec{B}$$

## Velocity Selector

> A device that filters charged particles, allowing only those with a specific velocity to pass through, while deflecting others  
> Particles with the correct velocity will have their electric and magnetic forces balanced, resulting in a straight path.

![](https://upload.wikimedia.org/wikipedia/commons/f/ff/Velocity_selector.svg)

$$
\begin{align}
F_{E}  & = qE  \\
F_{B}  & = q v B 
\end{align}
$$

For a particle to pass through undeviated, these forces must cancel exactly, which only happens for particles with a specific speed:

$$v=\frac{E}{B}$$

## Thomson's e/m Experiment

In 1897, J.J. Thomson used a cathode-ray tube with a velocity selector to measure the charge-to-mass ratio ($\frac{e}{m}$) of the electron. By finding the velocity of the electrons and then measuring their deflection in an electric field alone, he was able to calculate it, where V is the accelerating potential. This experiment led to the discovery of the electron.

$$
\frac{e}{m} = \frac{E^2}{2VB^2}
$$

![](https://upload.wikimedia.org/wikipedia/commons/thumb/a/a3/JJ_Thomson_Cathode_Ray_2_explained.svg/936px-JJ_Thomson_Cathode_Ray_2_explained.svg.png)

## Mass Spectrometer

This device identifies ions by their mass-to-charge ratio. Ions are first sent through a velocity selector to ensure they all have the same speed.

They then enter a region with only a magnetic field ($B^{'}$), where they follow a semicircular path. The radius of this path, is directly proportional to the ion's mass, allowing different isotopes or molecules to be separated and detected.

$$R=\frac{mv}{qB^{'}}$$

![](https://upload.wikimedia.org/wikipedia/commons/thumb/0/0d/Mass_Spectrometer_Schematic.svg/1280px-Mass_Spectrometer_Schematic.svg.png)

## Force and Torque on Conductors

The magnetic force on a wire is the sum of the forces on all the individual moving charges within it. For a straight conductor of length $l$ carrying current $I$ in a uniform field $B$, the net force is:

$$
F = I (l \times B)
$$

$l$ is a vector whose magnitude is the length of the wire and whose direction is along the current flow. For a wire that is not straight, the force must be found by integrating over infinitesimal segments:

$$
dF = I (dl \times B)
$$

## Torque on a Current Loop

When a closed loop of current is placed in a uniform magnetic field, the net force on it is zero, but it can experience a net **torque** that causes it to rotate.

To quantify this, we define the magnetic dipole moment (μ) of the loop:

$$
\mu = N I A
$$

N - Number of loops, **A is area vector**, perpendicular to the loop's plane (direction found via the right-hand rule).

---

The torque (τ) on the loop is given by:

$$
\tau = \mu \times B
$$

The potential energy (U) of this magnetic dipole in the field is:

$$
U = - \tau \cdot B
$$

The loop is in **stable equilibrium** when the torque is zero and the potential energy is at its minimum. This occurs when $\mu$ is parallel to $B$.

It is in unstable equilibrium when **torque is zero but potential energy is maximum**.

In a closed current loop within a uniform magnetic field, ==the net magnetic force is zero==.

---

**Why is there a net torque on a current loop in a uniform magnetic field, but no net force?**

In a uniform field, the forces acting on opposite sides of the loop are equal in magnitude and opposite in direction.

These opposing forces cancel each other out, resulting in zero net force.

==However, these forces do not act along the same line.== They form a "couple" that creates a turning effect, or torque, causing the loop to rotate until its magnetic moment aligns with the external field.
