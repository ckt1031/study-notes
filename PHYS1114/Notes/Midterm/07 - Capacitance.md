$$E = \frac{\sigma}{\epsilon_0} = \frac{Q}{A\epsilon_0}$$

## Capacitance

The standard method for calculating the capacitance of a given geometry involves a consistent four-step process:

- ==Assume a charge of magnitude $Q$ is placed on each conductor ($\pm Q$).==
- Use Gauss's Law to determine the electric field vector, $\vec{E}$, in the space between the conductors.
- Integrate the electric field along a path from the positive to the negative conductor to find the potential difference, $V_{ab}$.
- Apply the definition $C = Q/V_{ab}$ to find the capacitance.

We have a and b conductor, if a positive charge is moved from b to a, and there will be e-field towards conductor B.

$$
V \propto Q \quad C = \frac{Q}{V_{ab}}
$$

> Unit: **Farad** $1 F = 1 \frac{C}{V}$

If we have a light bulb between a and b connected in series, the positive charge will flow to B from A, negative charge flow from B to A, both conductor will be equalized, and when charge flowing bulb, there will be current offering power for bulb to light.

### Parallel-Plate Capacitor

$$
\begin{align}
V_{ab}  & = - \int^a_{b} \vec{E} \cdot d \vec{l} = \frac{\sigma}{\epsilon_{0}} d \\
 & = \frac{Q}{\epsilon_{0} A}d \\
C  & = \frac{Q}{V} = \frac{\epsilon_{0}A}{d}
\end{align}
$$

If I want to increase the charge with fixed voltage, I can increase the $C$, where I can either increase the area or decrease the distance between plates.

### Cylindrical Capacitor

A typical coaxial television cable has a capacitance of around **69 pF** per meter of length.

Inner radius $r_{a}$, outer radius $r_{b}$, total radius $R$.

$$
\begin{align} \\
\lambda L & = Q \\
V_{ab}  & = - \int^{r_{a}}_{r_{b}} \frac{\lambda}{ 2 \pi \epsilon_{0}} \frac{1}{r} dr \\
 & = \boxed{\frac{\lambda}{ 2 \pi \epsilon_{0}} \ln\left( \frac{r_{b}}{r_{a}} \right)} > 0 \\
C  & = \frac{Q}{\frac{Q}{L} \frac{1}{ 2 \pi \epsilon_{0}} \ln\left( \frac{r_{b}}{r_{a}} \right)} = \boxed{\frac{2 \pi \epsilon_{0} L}{\ln\left( \frac{r_{b}}{r_{a}} \right)}}
\end{align}
$$

### Spheral Capacitor

This geometry consists of two concentric spherical conducting shells with inner radius $r_a$​ and outer radius $r_{b}$​, at radius r where $r_{a} < r < r_{b}$

$$
\begin{align}
V_{ab}  & = - \int^{r_{b}}_{r_{a}} \frac{Q}{4 \pi \epsilon_{0} r^2} dr \\
 & = \frac{Q}{4 \pi \epsilon_{0}}  \left( \frac{1}{r_{a}} - \frac{1}{r_{b}}\right) \\
C  & = \frac{4 \pi\epsilon_{0}}{\left( \frac{1}{r_{a}} - \frac{1}{r_{b}}\right)} = \frac{4 \pi\epsilon_{0} \cdot r_{a} \cdot r_{b}}{\left( r_{b} - r_{a} \right)} \propto \frac{A \ (\text{Area})}{d}
\end{align}
$$

Consider big radii and small separation, $r_{a} \approx r_{b} \approx r$, $A \approx 4 \pi r^2$, ([[#Parallel-Plate Capacitor]])

$$
C \approx \epsilon_{0} \frac{A}{d}
$$

## Capacitors in Parallel

```tikz
\usepackage{circuitikz}
\begin{document}

\begin{circuitikz}[american, voltage shift=0.5]
\draw (0,0)
to[isource, l=$I_0$, v=$V_0$] (0,3)
to[short, -*, i=$Q$] (2,3)
to[C=$C_1$, i>_=$V$] (2,0) -- (0,0);
\draw (2,3) -- (4,3)
to[C=$C_2$, i>_=$V$]
(4,0) to[short, -*] (2,0);
\end{circuitikz}

\end{document}
```

Q between 1 and 2 is the same if their capacitance is the same.

$$
\begin{align}
V_{ab}  & = V_{1} = V_{2} = \dots = V_{n} \\
Q_{\text{Total}}  & = Q_{1} + Q_{2} + \dots + Q_{n} \\
C_{\text{eq}}  & = \frac{Q_{1} + Q_{2} + \dots + Q_{n}}{V_{ab}} = \frac{V_{ab} \cdot (C_{1} + C_{2} + \dots + C_{n})}{V_{ab}}  \\
& = \boxed{\sum_{i} C_{i}}
\end{align}
$$

## Capacitor in Series

```tikz
\usepackage{circuitikz}
\begin{document}
\begin{circuitikz}[american, voltage shift=0.5]
\draw (0,0)
to[isource,, v_=$V_0$] (6,0) % Changed from (0,6) to (6,0), added l_ and v_ for better placement
to[short, i_=$Q$] (6,2) % Changed from (2,6) to (6,2)
to[C=$R_1$, v_=$V_1$] (2.5,2) % Changed R=$C_1$ to R=$R_1$ for clarity and fixed v>_ to v_
to[C=$R_2$, v_=$V_2$] (0,2) -- (0,0); % Changed R=$C_2$ to R=$R_2$ and fixed v>_ to v_
\end{circuitikz}
\end{document}
```

By charge conservation, capacitor connected in series, number of charge along the same series must be the same.

$$
Q_{1} = Q_{2} = \dots = Q_{n}
$$

$$
C_{1} = \frac{Q}{V_{1}} \quad C_{2} = \frac{Q}{V_{2}}
$$

Their voltage is the **same** if and only if **their capacitance is the same**. (i.e. Area and distance)

$$
\begin{align}
V_{ab}  & = \frac{Q}{C_{\text{eq}}}  \\
V_{ab}  & = V_{1} + V_{2} + \dots + V_{n}\\
\frac{Q}{C_{eq}}  & = Q \cdot \left( \frac{1}{C_{1}} + \frac{1}{C_{2}} + \dots + \frac{1}{C_{n}} \right)  \\
\frac{1}{C_{eq}} & = \boxed{\sum_{i} \frac{1}{C_{i}}}
\end{align}
$$

## Energy Stored in Capacitors

This section *transitions* from the static property of capacitance to ==the dynamic process of storing energy.==

- Charging a capacitor requires work.
- An external agent, such as a battery, must move charge from one conductor to the other **against the opposing force of the electric field** that builds up as charge accumulates.

Consider moving an infinitesimal amount of positive charge, $dq$, from the *negative* plate to the **positive** plate. At a moment when the capacitor already holds a charge $q$, the potential difference across it:

$$
V = \frac{q}{C}
$$

The work done by electric field to move $dq$ across $V$:

$$
W = - V dq = - \frac{q}{C} dq
$$

The total work done to charge the capacitor from an uncharged state ($q=0$) to a final charge $Q$ is the **sum of all these infinitesimal increments**, found by integration:

$$
W = - \int^Q_{0} \frac{q}{C} \ dq = - \frac{Q^2}{2C} = - (U(Q) - U(0))
$$

If define $U(0) = 0$ (potential energy of an uncharged capacitor is zero)

$$
U = \frac{Q^2}{2C} = \frac{1}{2} CV^2 = \frac{1}{2} QV
$$

Energy stored isn't $QV$ since ==the voltage is not constant==, it increases as the charge accumulates, $\frac{1}{2}$ is the average voltage during the charging process.

- Changes when battery connect or disconnected

## Electric-Field Energy

Energy storage is distributed throughout the volume of space occupied **by the electric field created by the separated charges**.

This allows for the definition of an **energy density**, u, representing the amount of energy stored per unit volume.

For ideal plate-plate capacitor, the energy density $u$ is:

$$
\begin{align}
U  & = \frac{1}{2} \epsilon_{0} \frac{A}{d} (Ed)^2 =\frac{1}{2} \epsilon_{0} A E^2d \\
u  & = \frac{U}{Ad} = \frac{1}{2} \epsilon_{0} E^2
\end{align}
$$

This formula is universally applicable ==to any electric field in a vacuum==. It represents a fundamental principle: electric fields contain energy.

### Energy Stored in Spherical Conductor

$$
\begin{align}
C  & = \frac{4 \pi\epsilon_{0} \cdot r_{a} \cdot r_{b}}{\left( r_{b} - r_{a} \right)}  \\
U \text{(Work for Assemble charge)} & = \frac{Q^2}{2C} = \frac{Q^2 (r_{b} - r_{a})}{8 \pi \epsilon_{0} r_{a} r_{b}} \\
U \text{(Energy stored E-field)} & = \int^{r_{b}}_{r_{a}} \frac{1}{2} \epsilon_{0} E^2 4 \pi r^2 dr = \frac{Q^2 (r_{b} - r_{a})}{8 \pi \epsilon_{0} r_{a} r_{b}}
\end{align}
$$

Both methods yield the exact same result. This perfect agreement provides strong evidence that **associating energy with the field is a physically consistent and meaningful model**. It confirms that the energy required to assemble the charges is precisely equal to the ==total energy contained in the resulting electric field==.

## Applications of Network

- **Achieving High Capacitance**: If only small capacitance only, we can connect capacitors in ==parallel== to increase the total capacitance.
- **Achieving High Voltage**: In high-voltage circuits, the required operating voltage *may exceed the maximum rated (breakdown) voltage of any single capacitor*. Connected in ==series==, make voltage divided for smaller voltage for each.
- **Capacitive Voltage Dividers**: In AC circuits, capacitors in series act as a voltage divider. The voltage drop across any capacitor in the series is **inversely proportional to its capacitance** $V_1/V_2 = C_2/C_1$.

![image](https://obsidian-img-studies.tsun1031.xyz/2025/07/02/0c743874e208fe36a9fe518546c31db7.png)
