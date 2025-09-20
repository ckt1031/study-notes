$$
I_{Max} = Q_{0} \omega
$$

## Self-Induction and Inductors

When the current in a circuit changes, it creates a ==changing magnetic field==, which in turn induces an electromotive force in the same circuit. This phenomenon is called **self-induction**.

**Definition of Inductance:**

$$
L = \frac{N\Phi_{B}}{i}
$$

Inductance depends on the ==physical geometry of the coil==, such as its shape and number of turns. The SI unit for inductance is the Henry $\mathrm{1H = 1 T \cdot m^2/A}$.

### Self-Induced EMF

From Faraday's Law of Induction, the induced emf is the negative rate of change of magnetic flux, by substituting the definition of L, we get the equation for the self-induced emf in an inductor.

$$
\varepsilon = - N \frac{d \Phi_{B}}{dt} = - L \frac{di}{dt}
$$

An inductor produces an EMF that ==opposes any change in the current flowing through it==, a direct consequence of Lenz's Law.

### Inductors As Circuit Elements

**Potential Drop:** The voltage change is: $$V_{ba} = - L \frac{di}{dt}$$

If the current is **increasing** ($\frac{di}{dt} > 0$), there is a **potential drop** across the inductor in the direction of the current.

If the current is **decreasing** ($\frac{di}{dt} < 0$), there is a **potential rise** across the inductor in the direction of the current.

> If you traverse a circuit element in the direction _opposite_ to the current flow, the sign of the potential change is reversed.

## Magnetic Energy Storage

To establish a current in an inductor, ==an external power source must do work against the opposing self-induced EMF==. This work is stored as potential energy in the inductor's magnetic field.

### Derivation of Stored Energy

$$
U = \frac{1}{2} LI^2
$$

This is analogous to the energy stored in a capacitor, which is $U = \frac{1}{2} CV^2$

### Magnetic Energy Density

$$
u = \frac{B^2}{2 \mu_{0}} \quad \left( B=\frac{\mu_{0} Ni}{2 \pi r} \right)
$$

This general formula **applies to any magnetic field in a vacuum** and is analogous to the electric energy density in an electric field, $u_{E} = \frac{1}{2} \epsilon_{0} E^2$

$$
L = \frac{N \Phi_{B}}{i} = \frac{\mu_{0} N^2 A}{2 \pi r}
$$

## The R-L Circuit

An R-L circuit contains a ==resistor (R) and an inductor (L)==. The **inductor's opposition to changes in current** influences the circuit's behavior over time.

```tikz
\usepackage{circuitikz}
\begin{document}
\begin{circuitikz}[american voltages]
\draw (0,0)
  to[V, l=$V_s$] (0,2)      % Voltage source Vs
  to[R, l=$R$] (3,2)        % Resistor R
  to[L, l_=$L$] (3,0)       % Inductor L
  -- (0,0);                 % Wires to close the loop
\end{circuitikz}
\end{document}
```

### Current Growth

Assuming the initial current is zero.

$$
\begin{align}
\varepsilon - i R - L \frac{di}{dt}  & =0 \\
i(t)  & = \frac{\varepsilon}{R} (1- e^{-t/\tau}) \\
\tau  & = \frac{L}{R}
\end{align}
$$

The time constant $\tau$ represents the time it takes for the ==current to reach approximately 63%== (or $1-1/e$) of its final value.

**Final current**:

$$
I_{\text{Final}} = \frac{\varepsilon}{R}
$$

### Current Decay

If the circuit is already running with a steady current $I_{0}$ and the EMF source is suddenly removed, the inductor's stored energy causes the current to **decrease gradually rather than stopping instantly.**

For $\varepsilon =0$,

$$
- iR - L \frac{di}{dt} = 0
$$

$$
i(t) = I_{0} e^{-t/\tau}
$$

The time constant $\tau = L/R$ now represents the time it takes for the current to decay to about $37 \%$ (or $1/e$) of its initial value.

## The L-C Circuit: Electrical Oscillations

A circuit containing only an inductor (L) and a capacitor (C) **exhibits electrical oscillations**, where ==energy is continuously transferred between the capacitor's electric field== and the ==inductor's magnetic field==.

This system is a direct electrical analog to a mechanical mass-spring simple harmonic oscillator.

```tikz
\usepackage{circuitikz}
\begin{document}
\begin{circuitikz}[american voltages]
\draw (0,0)
  to[L, l=$L$] (3,0)      % Inductor L
  to[short] (3,2)        % Top wire
  to[C, l_=$C$] (0,2)      % Capacitor C
  -- (0,0);              % Bottom wire to close the loop
\end{circuitikz}
\end{document}
```

In an ideal L-C circuit, oscillations would continue forever because energy is perfectly conserved, shuttling between the capacitor and inductor.

However, any real circuit has _some resistance_ in its wires and components. This resistance dissipates energy as heat, **causing the oscillations to die out.** This leads to the R-L-C circuit model.

### Energy Transfer Cycle

![image](https://obsidian-img-studies.tsun1031.xyz/2025/07/24/c22e27d2747b0ac9bc61fed16f2ce4e1.png)

- $t=0$: A fully charged capacitor stores all the energy in its electric field ($U_{E}$​). Current is zero.
- $t=T/4$: **The capacitor fully discharges.** Current is now maximal, and all the energy is stored in the inductor's magnetic field ($U_{B}$).
- $t=T/2$: The **inductor's** collapsing magnetic field **recharges the capacitor with the opposite polarity.** All energy is back in the electric field.
- $t=3T/4$: The **capacitor** discharges again, creating a maximal current in the opposite direction. ==All energy is back in the magnetic field.==
- $t=T$: The cycle completes as the capacitor is fully recharged to its original state.

### Oscillation Equation

$$
\begin{align}
- L \frac{di}{dt} - \frac{q}{C} & = 0 \\
- L \frac{d^2q}{dt} - \frac{q}{C}  = 0 &  \implies L \frac{d^2q}{dt} + \frac{q}{C} = 0
\end{align}
$$

### Angular Frequency

$$
\begin{align}
q(t)  & = Q \cos(\omega t + \phi) \\
\omega  & = \sqrt{ \frac{1}{LC} } \sim \sqrt{ \frac{k}{m} } \ (\text{Mechanical}) \\
i (t)  & = Q \frac{d}{dt} \cos(\omega t + \phi) \\
 & = - Q \omega \sin (\omega t + \phi)
\end{align}
$$

## The R-L-C Circuit: Damped Oscillations

```tikz
\usepackage{circuitikz}
\begin{document}
\begin{circuitikz}[american voltages]
\draw (0,0)
  to[V, l=$V_s$] (0,2)      % Voltage source Vs
  to[R, l=$R$] (2,2)        % Resistor R
  to[L, l=$L$] (4,2)        % Inductor L
  to[C, l_=$C$] (4,0)       % Capacitor C
  -- (0,0);                 % Wires to close the loop
\end{circuitikz}
\end{document}
```

When a resistor (R) is added to an L-C circuit, **the energy is dissipated**, and the oscillations are damped. This is analogous to a damped mechanical oscillator.

$$
\begin{align}
- iR - L \frac{di}{dt} - \frac{q}{C}  & = 0 \\
\frac{d^2q}{dt^2} + \frac{R}{L} \frac{dq}{dt} + \frac{1}{LC} q  & = 0
\end{align}
$$

An ideal **LC circuit** will always oscillate, while an **RLC circuit** will only oscillate under certain conditions.  
The presence of the resistor ==determines whether the oscillations can occur or if they are suppressed.==

> An oscillation whose amplitude decays exponentially.

$$
A(t) = A_{0} e^{-\alpha t} \quad \alpha = \frac{R}{2L}
$$

![image](https://obsidian-img-studies.tsun1031.xyz/2025/07/24/1a25d82809c73e8f90a533cb0219653f.png)

### Damped Angular Frequency

The oscillation frequency is lowered by the resistance

$$
w^\prime = \sqrt{ \frac{1}{LC} - \frac{R^2}{4L^2}}
$$

### Types of Damping

#### Underdamped

$$
R < 2 \sqrt{ \frac{L}{C} }
$$

The circuit oscillates with a decaying amplitude. The charge $q$ varies.

#### Critically Damped

The system **returns to zero as quickly as possible without oscillating.**

$$
R = 2 \sqrt{ \frac{L}{C} }
$$

#### Over-damped

The system returns to zero slowly without oscillating.

$$
R > 2 \sqrt{ \frac{L}{C} }
$$
