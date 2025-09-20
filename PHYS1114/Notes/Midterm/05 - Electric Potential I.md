- Negative potential energy change implies a more stable system?

## Conservation of Electric Field

Consider a positive test charge $q_0$ moving in a uniform electric field $\vec{E}$.

The electric force on the charge is $\vec{F} = q_0 \vec{E}$.

The work done by this electric force as the charge moves a vertical distance $d$ from point a to point b is: $$W_{a \rightarrow b} = Fd = q_0 E d$$  
Just as with gravity, this work is independent of the path taken between $a$ and $b$.  

Consequently, ==the electric field is also conservative==, and we can define a change in electric potential energy $\Delta U$ such that: $$W_{a \rightarrow b} = - \Delta U_g$$

When the charge **moves in the direction of the electric force**, the field ==does positive work==, and the ==potential energy of the system decreases==. ($\Delta U < 0$).

The force $\vec{F}$ is purely radial, meaning $\vec{F} = F(r)\hat{r}$.

$$
\begin{align}
W_{a \rightarrow b}  & = \int^b_{a} F \cdot dl = \int^b_{a} F (r) \hat{r} \cdot dl = \int^{r_b}_{r_a} F (r) \cdot dr \\
& = \int^{r_b}_{r_a} \frac{1}{4\pi\epsilon_0} \frac{qq_0}{r^2} \cdot dr \\
 & = \frac{q q_{0}}{4\pi\epsilon_0} \left( \frac{1}{r_{a}} - \frac{1}{r_{b}} \right)
\end{align}$$

The work done depends only on the initial and final radial distances, $r_a$ and $r_b$, independent of path, confirming that the **electrostatic force is indeed conservative**.

Even if _a_ and _b_ not along the same radial line, work done formula is still the same, $dw = F dl \cos \phi = \vec{F} \cdot d \vec{r}$

## Electric Potential Energy

$$
\Delta U = U_{b} - U_{a} = - W_{{a\to b}}
$$

- When the field *does positive work* (e.g., as two like charges repel and fly apart), the system's potential energy is converted into another form, typically kinetic energy, and thus $\Delta U$ is negative.
- When an external agent does work against the field (e.g., pushing two like charges together), that work is stored as potential energy, and $\Delta U$ is positive.

To get absolute potential energy, it starts from 0, to infinite separation $\infty$.

$$
U(r) = W_{r\to \infty} = \frac{q q_{0}}{4\pi\epsilon_0} \left(\frac{1}{r} - \frac{1}{\infty} \right)= \frac{q q_{0}}{4\pi\epsilon_0} \frac{1}{r}
$$

$U(r)$ is the work that must be done by an external agent against the electric force to bring the test charge $q_0$ from infinity to the position $r$.

- For $U > 0$, like charges, $qq_0 > 0$, the force is repulsive. It must do positive work to **push the charges together from infinity**, storing energy in the system.
- For $U < 0$, un-like charges, $qq_0 < 0$, the force is attractive. As the charges are brought together from infinity, the electric field does positive work, and the potential energy of the system decreases, becoming negative.

## U of a Test Charge vs. U of a System

### Potential Energy of a Test Charge in a Field

This is how much potential energy does $q_0$ possess by virtue of its position in the field of the other charges?

$$
U = \frac{q_{0}}{4 \pi \epsilon_{0}} \sum_{i} \frac{q_{i}}{r_{i}}
$$

### Total Potential Energy of Assembling a System

- Bring $q_{1}$: No work done
- Bring $q_{2}$: Work is done against the field of $q_1$. $W_2 = \frac{1}{4\pi\epsilon_0} \frac{q_1 q_2}{r_{1,2}}$.
- Bring $q_{3}$: $W_3 = \frac{q_{3}}{4\pi\epsilon_0} \left( \frac{q_1}{r_{1, 3}} +  \frac{q_2}{r_{2, 3}}\right)$

$$
\begin{align}  
U & = W_1 + W_2 + W_3 +… \\  
 & = \frac{1}{4 \pi \epsilon_{0}} \sum_{i < j} \frac{q_{i} q_{j}}{r_{{i, j}}} \\  
 & = \frac{1}{2 \times4 \pi \epsilon_{0}} \sum_{i \neq j} \frac{q_{i} q_{j}}{r_{{i, j}}}  
\end{align}
$$

The condition $i<j$ is to ensure that the interaction energy for each pair (e.g., between $q_1$ and $q_2$) is **counted only once**.

## Electric Potential (V)

Voltage is scalar.

> $V=0$ does not necessarily implies $\vec{E} =0$

Electric potential is a a quantity describes the field itself, independent of any charge placed within it.

$$
V = \frac{U}{q_{0}}
$$

- Potential from a single point charge: $$V = \frac{1}{q_{0}} \left( \frac{1}{4 \pi \epsilon_{0}} \frac{qq_{0}}{r} \right) = \frac{1}{4 \pi \epsilon_{0}} \frac{q}{r}$$
- Potential from a system of point charges: $$V = \frac{1}{4 \pi \epsilon_{0}} \sum_{i} \frac{q_{i}}{r_{i}}$$
The unit of electric potential is the volt (V), named after Alessandro Volta, and is defined as one joule per coulomb ($1 \text{ V} = 1 \text{ J/C}$).

## Electron Volt

One electron-volt is the amount of energy gained or lost by a particle with charge equal in magnitude to the elementary charge $e$ when it **moves through** a potential difference of **one volt**.

$$
1 \text{eV} = 1.602 \times 10^{-19} \ \text{J}
$$

## Determining Potential from a Known Electric Field

$$
V_{ab} = V_{a} - V_{b} = \int^b_{a} \vec{{E}} \cdot d \vec{l} = - \int^a_{b} \vec{E} \cdot d \vec{l}
$$

For positive test charge, moving inwards **increases** voltage.
