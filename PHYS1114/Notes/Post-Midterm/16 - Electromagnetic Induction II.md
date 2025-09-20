
$$
B = \mu_{0} \frac{N}{L} I = \mu_{0} n I
$$

$$
\Phi_{B} = BA = \mu_{0} n IA
$$

$$
\varepsilon = \frac{d}{dt} BA = \mu_{0} n A \frac{dI}{dt}
$$

## Induced Electric Fields

A changing magnetic flux creates an induced electric field, which is responsible **for driving charge carriers around a loop**, even in the absence of a magnetic field at the location of the loop. This is a crucial concept because it introduces ==a non-electrostatic electric field.==

The induced E-Field is not electrostatic, $\Delta V \neq 0$

1. Induced electric field is not conservative (do not have a starting or ending point)
2. Electric potential is not defined for induced electric field
3. The conducting ring above is not equipotential surface ($\oint E \cdot dl\neq 0$).

$$
\begin{align}
\vec{J}  & = \sigma \vec{E} \\
\varepsilon = \oint \vec{E} \cdot d \vec{l}  & = \sum \Delta V \neq 0
\end{align}
$$

The work done by this field on a charge _q_ moving around a closed loop:

$$
W = q \oint E \cdot dl = q \mathcal{E}
$$

> The magnetic field is zero everywhere along the wire loop outside the solenoid.  
> Therefore, the magnetic force on the charge carriers in the ring is zero.

### Faraday's Law in terms of Induced Electric Field

$$
\oint E \cdot dl = - \frac{d\Phi_{B}}{dt}
$$

> The negative sign indicates that the induced electric field opposes the change in magnetic flux (Lenz's Law)

## Solenoid

![image](https://obsidian-img-studies.tsun1031.xyz/2025/08/01/3e9cd11ae59abc778d9d92c745887642.png)

### Outside the Solenoid ($r > R$)

$$
\begin{align}
E (2 \pi r)  & = - (\pi R^2) \frac{dB}{dt} \\
 E & = \boxed{- \frac{R^2}{2r} \frac{dB}{dt}} \propto \frac{1}{r}
\end{align}
$$

### Inside the Solenoid ($r < R$)

$$
\begin{align}
E ( 2 \pi r)  & = - (\pi r^2) \frac{dB}{dt} \\
E  & = \boxed{- \frac{r}{2} \frac{dB}{dt}} \propto r
\end{align}
$$

## Displacement Current and the Generalized Ampere's Law

$$
\oint B \cdot dl = \mu_{0} i_{encl}
$$

> Ampere's Law: only works for continuous currents.  
> When charging a capacitor, the **current is not continuous across the plates**, which creates a contradiction.  
> A real current $i_{C}$ flows through capacitor, but it **stops at the capacitor plates**, creating a discontinuity

- If we choose a flat surface cutting through the wire for our Amperian loop, the enclosed current is $i_{c}$.
- If we choose a bulging surface that passes between the capacitor plates, the enclosed **current is zero, leading to a contradiction**. Ampere's law predicts no magnetic field.

$$
\oint \vec{B} \cdot d \vec{l} = \mu_{0} \cdot I_{\text{Encl}} =0 \implies B =0
$$

To resolve this, James Clerk Maxwell introduced the concept of displacement current ($i_{D}$), a fictitious current that exists between the capacitor plates.

$$
\begin{align}
q  & = CV = \frac{\epsilon_{0}A}{d} Ed =EA \epsilon_{0} = \epsilon_{0} \Phi_{E} \\
i_{D}  & = \frac{dq}{dt} = \epsilon_{0} \frac{d\Phi_{E}}{dt} \\
i_{D}  & = \boxed{\epsilon_{0} \frac{d\Phi_{E}}{dt} }
\end{align}
$$

This displacement current **is not a flow of charge**, but a changing electric field that produces a magnetic field just as a real current does.

### Ampere-Maxwell Law

$$
\oint B \cdot dl = \mu_{0} (i_{c} + i_{D})_{\text{encl}} = \mu_{0} \left(i_{c} + \epsilon_{0} \frac{d\Phi_{E}}{dt}\right)_{\text{encl}}
$$

**Between plates** only $i_{D}$ is non-zero, Outside only $I_{C}$.

> The B field between the plates is due to changing electric flux, not magnetic flux.

### Measurable Consequences

**Inside the gap**:

$$
B(r) = \left( \frac{\mu_{0}}{2\pi} \frac{i_{c}}{R^2} \right)r
$$

**Outside the gap**:

$$
B (r) = \left( \frac{\mu_{0}i_{c}}{2\pi} \right) \frac{1}{r}
$$

## Induced E-Field Vs Induced B-Field
