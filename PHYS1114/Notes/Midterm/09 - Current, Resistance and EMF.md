An electric **current** is the net drift of charge from one location to another. In a conductive material like a metal wire, the outer electrons of the atoms are not bound to individual atoms but are free to move throughout the material.

- **Without an Electric Field:** These free electrons move randomly and chaotically, similar to gas molecules in a container. Their speeds are quite high (around $10^6$ m/s), but their directions are random, so there is no net flow of charge in any particular direction.
- **With an Electric Field**: When an external electric field ($E$) is applied across the conductor (for instance, by connecting it to a battery), the free electrons experience an electrostatic force ($F=qE$). Since electrons have a negative charge ($q = -e$), this force is in the direction opposite to the electric field. While their motion is still mostly random, this force gives them a small, net drift velocity ($v_{d}$) in a single direction. This collective drift constitutes the electric current.

It's important to note that the **conventional current** is defined as the direction that positive charge carriers would flow. Therefore, the direction of conventional current is opposite to the direction of the actual drift velocity of the electrons

## Current and Current Density

Current ($I$) is mathematically defined as the rate at which charge flows through a cross-sectional area of the conductor.

This macroscopic current to the microscopic drift velocity, consider a segment of wire with cross-sectional area A.

$$
I = \frac{dQ}{dt} = nq A v_{d}
$$

The SI unit for current is the **ampere (A)**, where 1 A = 1 coulomb per second.

---

**Current Density (J)** is a more general quantity that describes the current per unit cross-sectional area, removing the geometric dependency of the specific wire.

> Vector, pointing in the direction of conventional current.

$$
J = \frac{I}{A} = nqv_{d}
$$

## Ohm's Law, Resistivity, and Resistance

Materials that follow this are called **ohmic**, while those that don't are **non-ohmic**.

Resistivity $(\rho)$ is a measure of how strongly a material opposes the flow of electric current.

$$
J = \frac{E}{\rho}
$$

The reciprocal of resistivity is called **conductivity**.

### Resistance

For a uniform conductor of length L and cross-sectional area A:

$$
R = \rho \times\frac{ L}{A} \quad \left( 1 \Omega = 1 \frac{V}{A} \right)
$$

An **ohmic resistor** has a constant resistance, so its I-V graph is a straight line.

A **non-ohmic** device, like a semiconductor diode, has a *resistance that changes with voltage*, resulting in a curved I-V graph.

### Temperature Dependence of Resistance

**Metals**

As temperature increases, the metal's ions vibrate more vigorously. This increases the frequency of collisions with electrons, making it more difficult for them to drift and thus increasing resistivity.

$\alpha$ is the temperature coefficient of resistivity

$$
\begin{align}
\rho(T) & = \rho_{0} [1+\alpha ( T -T_{0})] \\
R(T) & = R_{0} [1+\alpha ( T -T_{0})]
\end{align}
$$

**Semiconductors**

In semiconductors, increasing the temperature excites more charge carriers into a conducting state, which generally *decreases* the resistivity.

**Superconductors**

Below a certain critical temperature ($T_{C}$​), the resistivity of a superconductor abruptly drops to zero.

## Electromotive Force (EMF)

An electric field in an isolated conductor will cause charges to move and accumulate at the ends. This buildup creates an opposing electric field, and very quickly, the net field inside becomes zero, stopping the current.

To maintain a steady current, two things are needed:

1. A complete, closed loop or **circuit**.
2. A device that provides an electromotive force (EMF or $\mathcal{E}$), such as a battery.

EMF is not a force, it represents the *work done per unit charge* to move charges from a lower potential to a higher potential, against the electrostatic force. The SI unit for EMF is the volt (V).

- An ideal EMF source has no internal energy loss. The terminal voltage ($V_{ab}$) across it is equal to its EMF: $V_{ab} = E$
- A real EMF source has an internal resistance (r). When it supplies a current I, some energy is dissipated within the source. The terminal voltage is then lower than the EMF:

$$V_{ab} = E - Ir$$

## Power in Electric Circuits

When a charge $dQ$ moves through a potential difference $V_{ab}$, the work done is $dW=V_{ab}dQ$.

Since $I=dQ/dt$, we can write $dQ=Idt$. The power $(P)$, which is the rate of doing work:

$$P=\frac{dW}{dt}=V_{ab}I$$

**Power Dissipated by a Resistor**

$$P = (IR)I = I^{2}R = R\frac{V_{ab}}{2}$$

**Power Delivered by an EMF Source**

$$P = V_{ab}I = (E - Ir)I = EI - I^{2}r$$

**Power for Charging a Battery**

$$P = V_{ab}I = EI + I^{2}r$$

## Resistors in Series

$$
R_{\text{Series}} = R_{1} + R_{2} + \dots = \sum_{i} R_{i}
$$

## Resistors in Parallel

$$
R_{\text{Parallel}} = \left( \frac{1}{R_{1}} + \frac{1}{R_{2}} + \dots \right)^{-1} = \left( \sum_{i} R_{i}^{-1} \right)^{-1}
$$
