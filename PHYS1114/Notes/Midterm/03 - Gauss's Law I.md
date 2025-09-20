## Electric Flux

> Electric flux is a measure of **the number of electric field lines** passing through a given surface.

- **Unit**: $\mathrm{N \cdot m^2 / C}$
- From positive to negative charges.
- For surface $\perp$ flow, the volume flow through after $dt$ is $A(v dt)$
- $\Phi =0$ when the flow is parallel to the surface.
- Surface at angle $\phi$, volume flow through after $dt$ is $A (v \ dt) \cos \phi = \vec{A} \cdot \vec{v} \ dt$
- Flux proportional to number of net charge inside.
- The flux is **independent to the size** of closed surface (as long as it encloses the same net charge)

### Net Flux and Enclosed Charge

- **Net Outward Flux**: More field lines exit than enter, indicating a net **positive charge is enclosed**.
- **Net Inward Flux**: More field lines enter than exit, indicating a net **negative charge is enclosed** ($Q_{\text{encl}} < 0$).
- **Zero Net Flux**: The number of field lines entering equals the number exiting. This occurs when the net enclosed charge is zero. Charges ==located _outside_ a closed surface== always produce zero net flux through that surface.

### Electric Flux of Uniform Field, Flat Surface

$$
\Phi_{E} = E \cdot A = EA \cos \phi
$$

### Electric Flux of Non-uniform Field and Curved Surface

$$
\begin{align}
\text{Non-uniform Field} &  : &  \Phi_{E} & = \int E  \cdot dA \\
\text{Closed Surface} &  : &  \Phi_{E} & = \oint E  \cdot dA
\end{align}
$$

The circle on the integral sign ($\, \oint \,$) signifies that the integration is performed over a complete, closed surface.

## Gauss's Law: A Fundamental Principle of Electrostatics

> Gauss's Law is one of the four Maxwell's equations.

> Gauss's Law states that the total electric flux through **any closed surface** (a "Gaussian surface") is ==directly proportional== to the net charge enclosed within that surface.

It does not work with **irregular shape and unknown charge distribution**.

$$
\begin{align}
\Phi &  = \oint E \cdot \ dA = \oint \vec{E} \cdot \ d \vec{A} = \oint E(r) \ dA \\
 & = E(r) \oint \ d A \\
 & = E(r) \cdot 4 \pi r^2 \\
 & =\frac{q_{\text{enclosed}}}{\epsilon_{0}} \propto q
\end{align}
$$

- This works for any shapes, even if the closed surface is not spherical, since we have $\vec{E} \ d \vec{A}$.

## Conductors in Electrostatic Equilibrium

A conductor is in **electrostatic equilibrium** when there is no net motion of charge within its volume or on its surface. This is a static condition, meaning that while charges may have moved to reach this state, all net charge flow (i.e., electric current) has ceased.

Net charge does not need to be zero, but it must be static.

![[03-electrostatic.excalidraw]]

### Property 1: The Electric Field Inside a Conductor is Zero

1. Electric field inside a conductor is $\mathbf{Zero}$, otherwise it will leads to a current inside the conductor.
	- if a non-zero electric field were to exist inside the conductor, it would exert a force ($\vec{F} = q\vec{E}$) on the free charges, causing them to accelerate and **constitute an electric current**.

### Property 2: Electric Field of a Conductor Must Be $\mathbf{\perp}$ to the Surface

If there were a component of the electric field parallel (tangential) to the surface, it would **exert a force** on the charges residing on the surface.

Thus, for the charges to be static, **the net force parallel to the surface must be zero**, which implies the electric field must be purely normal to the surface.

---

#### Why Wouldn't Charge Flies out from the Conductor Surface?

1. **Work Function (for Electrons)**
2. **Fixed Positive Ions (for "Positive Charges")**: The positive charges (atomic nuclei) are ==essentially fixed in the crystal lattice of the metal==.
3. However, there _is_ a point where the electric field becomes so incredibly strong that it _can_ cause charges to "fly out." This phenomenon is called **dielectric breakdown** (for the surrounding medium, like air) or **field emission** (for electrons directly from the metal surface).

### Property 3: Any Net Excess Charge Resides Entirely on the Conductor's Surface

$$
\vec{E} =0 \implies \Phi_{E} = 0 \implies Q_{\text{encl}} = 0
$$

The only way for the enclosed charge to be zero for any such surface is if there is no net charge anywhere within the volume of the conductor.

Therefore, any excess charge placed on the conductor cannot reside in its interior and must be located entirely on its surface.

## Hollow Conductors

> A hollow conductor is a conductor with an empty space inside it.

### Empty Cavity

If there is no charge within the cavity, the inner surface of the cavity can have no net charge.

Since $E=0$ everywhere on this surface, the net enclosed charge must be zero. As the cavity is empty, this **implies the charge on the inner surface is zero**. Any excess charge on the conductor resides on its outer surface.

### Charge Placed in Cavity

> The situation changes if a charge is introduced into the cavity (without touching the conductor).

If a point charge $+q$ is placed inside the cavity, it will induce an equal and opposite charge, $−q$, ==on the inner surface== of the conductor.

$$
Q_{\text{outer​}}=Q_C​−Q_{\text{inner}}
$$

If a hollow conductor with a net charge of $+7 \ \mathrm{nC}$ has a point charge of $-5 \ \mathrm{nC}$ placed in its cavity, a charge of $+5 \ \mathrm{nC}$ is induced on the inner wall. Leaving $+2 \ \mathrm{nC}$ on the outer surface.
