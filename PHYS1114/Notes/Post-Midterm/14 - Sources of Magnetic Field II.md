## Ampere's Law

Fundamental relationship between a magnetic field and the steady electric current that creates it.

It states that the line integral of the magnetic field ($\mathbf{B}$) around any arbitrary closed loop (an Amperian loop) is proportional to the total electric current ($I_\text{encl}$) passing through the surface enclosed by that loop.

$$
\oint B \cdot dl = \mu_{0} I_{\text{Encl}}
$$

- Holds for ==any steady, continuous current.==
- Only valid when ==no magnetic materials or time-varying electric fields are present.==
- Currents outside the Amperian loop do not contribute to the line integral.
- Ampere's Law is most useful for calculating the magnetic field ($B$) in situations with high symmetry.

## Applications of Ampere's Law

### Magnetic Field of a Long Straight Conductor

Due to cylindrical symmetry, the magnetic field ($\mathbf{B}$) is constant in magnitude along this path and is always parallel to the path element d$\mathbf{l}$.

$$
\begin{align}
B \oint dl  & = \mu_{0} I \\
B (2 \pi r)  & = \mu_{0} I \\
 B & = \boxed{\frac{\mu_{0} I}{2 \pi r}}
\end{align}
$$

For current density:

$$
\begin{align}
J  & = \frac{I}{A} = \frac{I}{\pi r^2} \\
B &  = \frac{\mu_{0} J \pi r^2}{2 \pi r} = \boxed{\frac{\mu_{0} J r}{2}}
\end{align}

$$

### Magnetic Field of a Long Cylindrical Conductor

Consider a cylindrical conductor of radius R carrying a total current I.

#### Outside the Conductor ($r>R$)

The derivation is identical to that of a long straight wire. The Amperian loop encloses the entire current I.

$$
B = \frac{\mu_{0}I}{2\pi} \frac{1}{r} \propto \frac{1}{r}
$$

#### Inside the Conductor ($r<R$)

Assuming a uniform current density:
$$
I_{\text{Encl}} = I \left( \frac{\pi r^2}{\pi R^2} \right) = I \frac{r^2}{R^2}
$$

$$
\begin{align}
B (2 \pi r)  & = \mu_{0} I_{\text{Encl}} \\
B  & = \frac{\mu_{0}}{2 \pi r} I \frac{r^2}{R^2} \\
 & = \boxed{\frac{\mu_{0} I}{2 \pi}  \frac{r}{R^2}} \propto \frac{r}{R^2}
\end{align}
$$

### Magnetic Field of a Solenoid

A solenoid is a coil of wire wound into a long cylinder. For an ideal, long solenoid, the magnetic field **is assumed to be uniform inside and zero outside.**

- We use a rectangular Amperian loop with one side of length $L$ inside the solenoid and the parallel side outside.
- The integrals along the sides **perpendicular to the solenoid axis cancel out**, $\oint B \cdot dl$ is zero since $B=0$.
- The only non-zero contribution is ==from the segment of length L inside the solenoid==, which gives $BL$. (The magnetic field outside the solenoid is assumed to be zero)
- The enclosed current is the number of turns within the length L, which is N, multiplied by the current I in each turn. So, $\boxed{I_{\text{Encl}}=NI}$.

$$
B = \frac{\mu_{0}NI}{L} = \mu_{0} n I \quad(n=\text{number of turns per unit length})
$$

### Magnetic Field of a Toroidal Solenoid (Toroid)

A toroid is essentially **a solenoid bent into a donut shape**. The magnetic field is confined almost entirely within the windings.

$B$ is constant along this path by symmetry, $\oint B \cdot dl = B (2 \pi r)$.

$$
B = \frac{\mu_{0} NI}{2 \pi r}
$$

Note that unlike an ideal solenoid, the magnetic field inside a toroid is not uniform. It varies with the radial distance $r$.

### Coaxial Cable

The magnetic field outside the cable is **zero**.

According to Ampere's law, an Amperian loop drawn outside the entire cable encloses two currents that are equal in magnitude and opposite in direction.

Therefore, the net enclosed current ($I_{\text{encl}}$) is zero, which means the line integral of the magnetic field is **zero**, and thus the magnetic field itself must be **zero**.

## Magnetic Materials

$$
B = \mu_{0} (H + M)
$$

Materials respond to **external magnetic fields** based on the magnetic properties of their atoms. Atomic electrons create ==microscopic current loops, giving rise to magnetic dipole moments ($\mu$)==.

### Magnetization

Total magnetic dipole moment per unit volume of a material. Measure of **how strongly a material responds to an applied magnetic field.**

$$
M = \frac{\mu_{\text{Total}}}{V}
$$

### Paramagnetism 順磁性

Paramagnetic materials are ==weakly attracted== to external magnetic fields, **increase** the magnetic field.

Individual atoms have **a net non-zero magnetic moment** ($\mu_{\text{Atom}} \neq 0$).

In the absence of an external field, these moments **are randomly oriented**, and the net magnetization is zero.

When an external field $B_{0}$ is applied, the atomic moments tend to align with the field to minimize their potential energy ($U = - \mu_{\text{Atom}} \cdot B_{0}$), creating a net magnetization ($M$) in the same direction as the external field.

---

**Why is paramagnetism a weak phenomenon?**

The magnetic potential energy gained by aligning an atom with a typical external field is ==significantly smaller than the average thermal kinetic energy of the atom at room temperature== ($U_m \ll K$). The randomizing effect of thermal motion makes it very difficult for the moments to become fully aligned with the field.

### Diamagnetism 抗磁性

Diamagnetic materials are **repelled by external magnetic fields**, slightly **decrease** the magnetic field.

In these materials, atoms have no net magnetic moment ($\mu_{\text{atom}} = 0$). However, when an external field is applied, it induces a magnetic moment within the atoms that, according to Lenz's law, ==opposes the external field==.

This induced opposing field **causes the total magnetic field inside the material to decrease**. This results in relative permeability $K_m < 1$ and small negative magnetic susceptibility $\chi_m < 0$.

All materials exhibit diamagnetism, but it is often masked by stronger paramagnetic or ferromagnetic effects.

### Ferromagnetism 鐵磁性

Ferromagnetic materials, like *iron and nickel*, exhibit **a strong attraction to magnetic fields**, **increase** the magnetic field.

Ferromagnetism arises from ==a quantum mechanical interaction== that causes the magnetic moments of neighboring atoms to align ==spontaneously==, forming large regions called **magnetic domains**. Within each domain, all magnetic moments are parallel. In an unmagnetized material, the domains are randomly oriented, resulting in no net magnetization.

**Effect in an External Field**:

- In a weak external field, domains aligned with the field grow by moving the domain walls.
- In a stronger field, the domains themselves rotate to align with the field.
- This results in a very large net magnetization and a tremendous increase in the magnetic field inside the material, with relative permeabilities $K_{M} \sim 10^3 \ \text{to} \ 10^5$.

#### Hysteresis 磁滯現象

Once magnetized, a ferromagnetic material ==retains some magnetization even after the external field is removed.==

A reverse field must be applied to bring the magnetization back to zero.

The enclosed area in a hysteresis loop represents the energy lost during a magnetization-demagnetization cycle.

- **Hard Magnets:** Materials with **wide hysteresis loops** are difficult to magnetize and demagnetize, making them suitable for permanent magnets and memory storage.
- **Soft Magnets:** Materials with ==narrow hysteresis loops lose little energy==, making them ideal for electromagnets, motors, and transformers.

![image](https://obsidian-img-studies.tsun1031.xyz/2025/07/24/743b180648a4ca193d7739c456bbad07.png)
