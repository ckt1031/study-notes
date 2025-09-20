Electromagnetic induction is the phenomenon where a **changing magnetic environment** creates an EMF in a conductor, such as a wire coil. This induced EMF can then drive an electric current.

$$
\varepsilon = \frac{1}{2} B \omega L^2
$$

## Faraday's Law of Induction

Induced EMF in any closed circuit is equal to the negative of the time rate of change of the magnetic flux through the circuit.

$$
\begin{align}
\varepsilon  & = - \frac{d\Phi_{B}}{dt} \\
\Phi_{B}  & = \int B \cdot dA
\end{align}
$$

$$
\begin{align}
\varepsilon  & = - \frac{\Delta \Phi_{B}}{dt}
\end{align}
$$

## Lenz's Law

Lenz's Law gives its **direction**.

> The direction of the induced current is such that it creates a magnetic field that **opposes the change in magnetic flux** that produced it.

- If the magnetic flux through a loop is  **increasing**, the induced current will generate a magnetic field in the **opposite direction** to the original field.
- If the magnetic flux is **decreasing**, the induced current will generate a magnetic field in the **same direction** as the original field to try and counteract the decrease.

## Applications

### AC Generator (Alternator)

A simple alternator consists of a loop of wire rotating with a **constant angular speed** ($\omega$) in a **uniform magnetic field** ($B$).

> The magnetic flux $\Phi_{B}$ changes not because the field or area changes, but because the angle ($\phi$) between $\mathbf{B}$ and the area vector $\mathbf{A}$ changes continuously.

$$
\begin{align}
\phi  & = \omega t \\
\Phi_{B}  & = BA \cos(\omega t) \\
\varepsilon  & = - \frac{d}{dt} (BA \cos(\omega t)) \\
 & = BA \omega \sin(\omega t)
\end{align}
$$

> The EMF is zero when the flux is at its maximum or minimum.

### DC Generator and Motors

This is similar to an alternator but uses a **commutator** (a split-ring) to reverse the connection to the external circuit every half-rotation.

$$
\varepsilon = \omega BA \left| \sin (\omega t) \right|
$$

---

When an external voltage drives a current through the motor's coil, the coil spins. As it spins in the magnetic field, it induces its own "back EMF" that **opposes the external voltage**.

> Why do the lights in your house sometimes dim when a large appliance like a refrigerator turns on?

When the motor first starts, its rotational speed ($\omega$) is near zero. Therefore, the back EMF ($E_\text{back} \propto \omega$) is also near zero.

With **very little back EMF to oppose the applied voltage**, a very large current is drawn from the house's circuit, causing a momentary voltage drop that dims the lights. As the motor gets up to speed, the back EMF increases, and the current drawn decreases to a normal operating level.

$$
I = \frac{V_{\text{supplied} } - V_{\text{Back}}}{R}
$$

## Slide-Wire Generator (Faraday's "rail gun")

$$
\varepsilon = BL v
$$

**Magnetic** force $F=BIL$ opposes motion

**Mechanical** power $Fv= I \varepsilon$ equals electrical power dissipated → energy conservation.

## Flux Change by Deforming Loops

Squeezing a loop in constant $\mathbf{B}$ decreases area $\mathbf{A}$ $\Rightarrow$ flux drops $\Rightarrow$ EMF appears only while area changes. Final EMF is zero once shape is fixed.

## Superconductors

In a hypothetical superconducting loop ($R=0$), Lenz's law implies that the loop will completely resist any change in flux.

An induced "persistent current" will perfectly cancel out any change, keeping the total flux through the loop constant.
