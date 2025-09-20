Dielectrics 電介質 explains how inserting a non-conducting material into a capacitor **enhances its performance.**

In practical capacitors, the space between the conducting plates is ==rarely a vacuum==.

It is typically filled with an insulating material known as a **dielectric**, such as plastic, glass, mica, or even purified water.

1. **Structural Support:** They provide physical separation and rigidity, preventing the conductors from touching.
2. **Increased Breakdown Voltage:** Most dielectric materials can ==withstand a much stronger electric field== than air before they ionize and become conductive. This property, called **dielectric strength**, allows a capacitor to be operated at a higher voltage without failure, thereby storing significantly more energy.
3. **Increased Capacitance:** For a given voltage, a capacitor with a dielectric can store more charge than the same capacitor with a vacuum between its plates.

$Q$ remains constant, voltage $V$ decreases due to the increased capacitance $C$.

A dielectric material will ==decrease the strength of an external electric field passing through it==. This happens because the external field causes a ==polarization== within the dielectric, creating an internal electric field that opposes the external one.

## The Dielectric Constant

> This is to measure how much a dielectric material increases the capacitance of a capacitor compared to a vacuum.

Since adding dielectric increases the capacitance, it must be greater than one.

$$
K = \frac{C}{C_{0}} > 1
$$

For $Q$ is constant, the voltage $V$ across the capacitor decreases by a factor of $K$:

$$
V = \frac{Q}{C} = \frac{Q}{KC_{0}} = \frac{V_{0}}{K}
$$

Where $C_0$ is the capacitance of the capacitor without the dielectric in vacuum.

## Permittivity of the Material

$$
\epsilon = K \epsilon_{0}
$$

With this definition, all the vacuum-based formulas for capacitance can be adapted for use with dielectrics simply by replacing the permittivity of free space, $\epsilon_0$, with the material's permittivity, $\epsilon$.

$$
\begin{align}
C  & = \frac{\epsilon A}{d} \\
u  & = \frac{1}{2} \epsilon E^2
\end{align}
$$

**Gauss's Law** is also modified for dielectrics. It's important to distinguish between **free charges** (on the conductors) and **bound charges** (induced on the dielectric).

$$
\oint KE \cdot \mathrm{d} A = \frac{Q_{\text{Encl - Free}}}{\epsilon_{0}}
$$

## Dielectric Strength

The maximum field a dielectric can sustain before breakdown is called the **dielectric strength**.

Under a strong electric field, a dielectric may be partially ionized and becomes conducting, called **dielectric breakdown**, e.g., corona discharge, or even lightning, is the dielectric breakdown of air.

When dielectric breakdown occurs, the dielectric material becomes conductive, and the capacitor can ==no longer function as intended==, leading to a short circuit or failure.

| Material                 | Dielectric Constant, K | Dielectric Strength, Em​ ($\mathrm{V/m}$) |
|:----------------------- |:--------------------- |:---------------------------------------- |
| Vacuum                   | $1$                    | $\infty$                                  |
| Air ($1 \ \mathrm{atm}$) | $1.00059$              | $3 \times 10^6$                           |
| Polypropylene            | $2.2$                  | $7 \times 10^7$                           |
| Teflon                   | $2.1$                  | $6 \times 10^7$                           |
| Pyrex glass              | $4.7$                  | $1 \times 10^7$                           |
| Water (pure)             | $80.4$                 |???                                       |
| Strontium Titanate       | $310$                  | $8 \times 10^6$                           |

Pure water has large dielectric constant, but dissolved impurities conduct electricity easily making it unsuitable for capacitors.

A high dielectric constant ==does not guarantee high dielectric strength.==

## Induced Charge and Electric Field Reduction

When a dielectric is placed in an electric field, it becomes polarized, and charges are induced on its surface.

**Polar Molecules**: These molecules have a permanent dipole moment. In the absence of an electric field, they are *oriented randomly*. When an external field is applied, they tend to align with the field, creating an induced surface charge.

**Nonpolar Molecules**: These molecules do not have a permanent dipole moment. An external electric field causes a slight separation of their positive and negative charges, inducing a dipole moment. This polarization also leads to an induced surface charge.

---

This induced surface charge ($\sigma_{i}$) creates an electric field within the dielectric that opposes the original external field ($E_{0}$). **The net electric field ($E$) inside the dielectric is therefore weaker than the field in a vacuum.**

The relationship between the original field and the net field is given by:

$$
\begin{align}
E  & = \frac{E_{0}}{K} \\
\sigma_{i}  & = \sigma \left( 1 - \frac{1}{K} \right)
\end{align}
$$

## Energy Storage in Capacitors with Dielectrics

The energy stored in a capacitor is affected by ==the presence of a dielectric==, and the outcome depends on the conditions under which the dielectric is inserted.

### Case 1: Constant Charge (Isolated Capacitor)

If a charged capacitor is disconnected from its charging source (constant *$Q$*), and then a dielectric is inserted, the voltage drops to $V = V_{0}/K$. The stored energy *U* decreases:

$$
U = \frac{1}{2} CV^2 = \frac{1}{2} (KC_{0})\left( \frac{V_{0}}{K} \right)^2 = \frac{1}{K} \left( \frac{1}{2} C_{0} V_{0}^2 \right) = \frac{U_{0}}{K}
$$

As the dielectric is inserted, the fringe electric fields at the edges of the capacitor plates polarize the dielectric and pull it in. **The electric field does positive work on the dielectric**, and this work accounts for the decrease in the potential energy stored in the capacitor $W = -\Delta U$

### Case 2: Constant Voltage (Capacitor Connected to a Battery)

If the capacitor remains connected to the battery (constant $V$), inserting a dielectric increases the capacitance to $C = KC_{0}$. The stored energy *U* increases:

$$
U = \frac{1}{2} (K C_{0}) V^ 2 = KU_{0}
$$

**This addresses the seeming paradox**: while an isolated capacitor loses energy, a capacitor kept at a constant voltage can store *more* energy with a dielectric.
