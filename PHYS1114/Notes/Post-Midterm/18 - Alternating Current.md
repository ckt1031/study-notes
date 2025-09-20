## Alternating Current (AC)

An alternating current (AC) source supplies a voltage **that varies sinusoidally over time.**

Instantaneous voltage:

$$
v = V \cos(\omega t)
$$

Frequency:

$$
\omega = 2 \pi f \quad T = f^{-1}
$$

For instance, in Hong Kong, the standard frequency is 50 Hz, which corresponds to an angular frequency of approximately 314 rad/s.

## Phasor Diagrams

A phasor is a **rotating vector** used to represent a sinusoidal quantity like an alternating current or voltage. This graphical representation simplifies the analysis of AC circuits, especially when multiple signals are involved.

- The **length of the phasor** represents the maximum current, _I_.
- The phasor **rotates counterclockwise** with an angular speed _ω_ equal to the angular frequency of the signal.
- The **projection of the phasor onto the horizontal axis** at any time _t_ gives the instantaneous current _i_ at that moment.

The main advantage of using phasor diagrams is that they allow for the addition of multiple sinusoidal signals of the same frequency through simple vector addition, ==avoiding the complexity of drawing and summing multiple sine waves.==

## Root-Mean-Square (RMS) Values

**The average value** of a sinusoidal signal over one period **is zero**, which is not a useful measure. To describe the effective value of an AC current or voltage, the **root-mean-square (RMS)** value is used.

$$
\begin{align}
i  & = I \cos (\omega t) \\
i^2  & = I^2 \cos^2 (\omega t) \\
(i^2)_{\text{avg}}  & = I^2 \cos^2 (\omega t)_{\text{avg}} = \frac{I^2}{2} \\
I_{\text{rms}}  & = \frac{I}{\sqrt{ 2 }}
\end{align}
$$

$$
V_{\text{rms}} = \frac{V}{\sqrt{ 2 }}
$$

## AC Circuits with Single Elements

### Resistor in an AC Circuit

When an AC current $i=I\cos(\omega t)$ flows through a resistor, the instantaneous voltage across the resistor:

$$
v_{R} = i R = (IR) \cos (\omega t )
$$

```tikz
\usepackage{circuitikz}
\begin{document}
\begin{circuitikz}[american voltages]
\draw (0,0)
  to[sinusoidal voltage source, l=$v_s(t)$] (0,2)  % AC voltage source
  to[R, l=$R$] (3,2)                             % Resistor R
  -- (3,0)                                       % Connecting wire
  -- (0,0);                                      % Close the loop
\end{circuitikz}
\end{document}
```

**Maximum voltage**

$$
V_{R} = IR
$$

- **Phase:** The voltage and current are **in phase**. This means their peaks and troughs occur at the same time.  
- **Phasor Diagram:** The voltage and current phasors are collinear and rotate together.

### Inductor in an AC Circuit

```tikz
\usepackage{circuitikz}
\begin{document}

\begin{circuitikz}[american voltages]
\draw (0,0)
  to[sinusoidal voltage source, l=$v_s(t)$] (0,2)  % AC voltage source
  to[L, l=$L$] (3,2)                              % Inductor L
  -- (3,0)                                        % Connecting wire
  -- (0,0);                                       % Close the loop
\end{circuitikz}

\end{document}
```

For an inductor, the voltage is proportional to the rate of change of the current:

$$
v_{L} = L \frac{di}{dt} = L \frac{d}{dt} (I \cos (\omega t)) = - I \omega L \sin (\omega t) = I \omega L \cos \left( \omega t + \frac{\pi}{2} \right)
$$

- **Phase:** The voltage across the inductor **leads** the current by $90^\circ$.
- **Inductive Reactance ($X_L$)**: This is the opposition to the current flow, defined as $X_L = \omega L$.
	- SI unit is the Ohm ($\Omega$). The maximum voltage is $V_L = IX_L$.

### Capacitor in an AC Circuit

```tikz
\usepackage{circuitikz}
\begin{document}

\begin{circuitikz}[american voltages]
\draw (0,0)
  to[sinusoidal voltage source, l=$v_s(t)$] (0,2)  % AC voltage source
  to[C, l=$C$] (3,2)                              % Inductor L
  -- (3,0)                                        % Connecting wire
  -- (0,0);                                       % Close the loop
\end{circuitikz}

\end{document}
```

For a capacitor, the voltage is proportional to the charge $v_C = q/C$, and the current is the rate of change of charge $i=dq/dt$.

$$
v_{C} = \frac{q}{C} = \frac{1}{C} \int i \ dt= \frac{1}{C} \int I \cos(\omega t) \ dt = \frac{I}{\omega C} \sin (\omega t) = \frac{I}{\omega C} \cos \left( \omega t - \frac{\pi}{2} \right)
$$

- **Phase:** The voltage across the capacitor **lags** the current by $90^\circ$ ($-\pi/2$ radians).
- **Capacitive Reactance ($X_C$):** This is the opposition to current flow, defined as $X_C = 1/(\omega C)$.
	- $\text{SI}$ unit is also the Ohm ($\Omega$). The maximum voltage is $V_C = IX_C$.

### Frequency Changes

An AC voltage of fixed amplitude is applied across a circuit element. If the frequency $f$ is increased, what happens to the amplitude of the current if the element is an inductor? What if it's a capacitor?

$$
\begin{align}
X_{L}  & = \omega L \\
I  & = \frac{V}{X_{L}} \quad (\omega \uparrow \implies I \downarrow) \\
I  & = \frac{V}{X_{C}} = V \omega C  \quad (\omega \uparrow \implies I \uparrow)
\end{align}
$$

## The L-R-C Series Circuit

The instantaneous voltage from the source is the sum of the voltages across each component:

```tikz
\usepackage{circuitikz}
\begin{document}
\begin{circuitikz}[american voltages]
\draw (0,0)
  to[sinusoidal voltage source, l=$v_s(t)$] (0,2)      % Voltage source Vs
  to[R, l=$R$] (2,2)        % Resistor R
  to[L, l=$L$] (4,2)        % Inductor L
  to[C, l_=$C$] (4,0)       % Capacitor C
  -- (0,0);                 % Wires to close the loop
\end{circuitikz}
\end{document}
```

$$
v = v_{R} + v_{L} + v_{C}
$$

- $V_R$ is in phase with the current $I$.
- $V_L$ leads $I$ by $90^\circ$.
- $V_C$ lags $I$ by $90^\circ$.
- $V_{L}$ and $V_{C}$ are antiparallel.

### Impedance (Z)

$$
\begin{align}
V  & = \sqrt{ V^2_{R} + (V_{L} - V_{C})^2 } \\
 & = I \sqrt{ R^2 + (X_{L} - X_{C})^2 } \\
 & = I Z \\
Z & = \sqrt{ R^2 + \left(\omega  L- \frac{1}{\omega C} \right)^2 }
\end{align}
$$

How if the AC frequency becomes very large?

$$
I_{\text{rms}} = \frac{V_{\text{rms}}}{Z} \quad (\omega \uparrow \implies Z \uparrow \implies I \downarrow)
$$

### Phase Angle

- If $X_L > X_C$, $\phi$ is positive, and the voltage **leads** the current (the circuit is inductive).
- If $X_L < X_C$, $\phi$ is negative, and the voltage **lags** the current (the circuit is capacitive).

$$
\begin{align}
\tan \phi = \frac{V_{L} - V_{C}}{V_{R}} = \frac{I(X_{L} - X_{C})}{IV_{R}}= \frac{X_{L} - X_{C}}{R} 
\end{align}
$$

## Power in AC Circuits

The instantaneous power delivered by the source is $p=vi$. The average power is the most useful measure.

- **Resistor**: The average power dissipated.
- **Inductor and Capacitor:** The average power delivered to an ideal inductor or capacitor ==over a full cycle is zero==. They store energy during one part of the cycle and return it to the circuit in another.

For the **entire L-R-C circuit**, the average power is given by:

$$
(p)_{\text{av}} = \frac{1}{2} VI \cos (\phi) = V_{\text{rms}} I_{\text{rms}} \cos (\phi)
$$

The term $\cos (\phi)$ is called the **power factor**. It represents the fraction of the apparent power that is actually dissipated as heat. From the impedance triangle (derived from the phasor diagram), we can see:

$$
\cos (\phi) = \frac{R}{Z}
$$
==Maximum power== is delivered when $\cos(\phi)=1$, which occurs when $Z = R$.

## Resonance in AC Circuits

Resonance occurs in an L-R-C circuit when the **inductive reactance equals the capacitive reactance** ($X_L=X_C$).

At this point, the impedance _Z_ is at its ==minimum== value $Z=R$.

This allows the current amplitude $I$ to reach its ==maximum== for a given source voltage V ($I=V/R$).

$$
\phi = 0 \quad \cos \phi =1
$$

The **resonance angular frequency**, $\omega_0$, is the frequency at which this occurs:

$$
X_{L} = X_{C} \implies \omega_{0} L = \frac{1}{\omega_{0} C} \implies \omega_{0} = \frac{1}{\sqrt{ LC }}
$$

The sharpness of the resonance peak depends on the resistance R, ==a smaller R results in a sharper and higher peak==. This principle is fundamental to tuning circuits, like in a radio.

## Key Differences Between Resistance (R) and Reactance (X)

Reactance refers to ==the opposition to the flow of alternating current (AC)== caused by inductors and capacitors.

- **Resistance (R)** dissipates energy, converting electrical energy into heat. This energy is permanently removed from the circuit.
- **Reactance (X)**, found in ideal inductors and capacitors, stores energy and later returns it to the circuit. The average power consumed by an ideal reactive component over a full cycle is zero.
