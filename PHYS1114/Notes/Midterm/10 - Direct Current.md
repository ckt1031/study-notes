## Kirchhoff's Junction Rule

This rule is a statement of the **conservation of charge**. It dictates that charge cannot accumulate at a junction. *Therefore, the total current flowing into a junction must equal the total current flowing out of it.*

$$
\sum_{i} I_{i} = 0
$$

A common sign convention is to treat current flowing into a junction as negative and current flowing out as positive.

$$
I_{3} = I_{2} + I_{1}
$$

## Kirchhoff's Loop Rule

This rule stems from the **conservation of energy**. It states that the algebraic sum of the potential differences (voltages) around any closed loop in a circuit must be zero. This is because the electric potential at any single point in the circuit is constant.

$$
\sum_{i} V_{i} = 0
$$

### EMF (Voltage Source)

- If you travel from the negative to the positive terminal, the potential change is $+ \ \mathcal{E}$.
- If you travel from the positive to the negative terminal, the potential change is $+ \ \mathcal{E}$.

### Resistor

- If you travel in the **same direction** as the current, the potential change is $-IR$ (a potential drop).
- If you travel in the **opposite direction** to the current, the potential change is $+IR$ (a potential rise).

## R-C Circuits: Charging a Capacitor

An R-C circuit contains a resistor and a capacitor. When a switch is closed to connect an initially uncharged capacitor to a battery, the capacitor begins to charge.

![image](https://obsidian-img-studies.tsun1031.xyz/2025/07/02/da6d99c871ea8e18f2403664f4693770.png)

|                  | At time 0          | After a long time         |
| ---------------- | ------------------ | ------------------------- |
| Current          | $\varepsilon - IR$ | $0$                       |
| Charge in C      | $0$                | $q=Q_{f} = C \varepsilon$ |
| Voltage across C | $V = \frac{q}{C}$  | $V = \varepsilon$         |

![image](https://obsidian-img-studies.tsun1031.xyz/2025/07/13/ed72a7924bf000390053b8683ef3a2b3.png)

---

$$
\begin{align}
\mathcal{E} - I R - \frac{q}{C} & = 0
\end{align}
$$

$$
\begin{align}
\epsilon - R \frac{dq}{dt} - \frac{q}{C} & = 0 \\
  \implies Q_{f} - q  & = RC \cdot \frac{dq}{dt} \\
  \implies \frac{dq}{Q_{f} - q}  &  = \frac{dt}{RC} \\
  \implies \int^{q(t)}_{{q(0) = 0}} \frac{dq}{Q_{f} - q}  &  = \int^t_{0} \frac{dt}{RC} \\
  \implies \frac{t}{RC}  & = \ln\left( \frac{Q_{f} }{Q_{f} - q(t)} \right)  \\
 \\
e^\frac{t}{RC}  & = \frac{Q_{f} }{Q_{f} - q(t)} \\
q(t)  & = - \frac{Q_{f} - e^\frac{t}{RC} \cdot Q_{f}}{e^\frac{t}{RC}} = \boxed{Q_{f} \cdot ( 1 - e^{-\frac{t}{RC}} )}
\end{align}
$$

### Time Constant

> The time taken to either increase to a factor ($1- \frac{1}{e}$) of the final value

$$
\tau = RC
$$

So to increase the speed to charge up the capacitor, decrease the time constant.

### Current by time

$$
\begin{align}
i(t)  & = \frac{\epsilon}{R} e^{-t/RC} = i(0) \cdot e^{-t/RC} 
\end{align}
$$

### Power Delivery

Instantaneous power:

$$
\begin{align}
i(t) \cdot \epsilon - i(t)^2 \cdot R - i(t) \left( \frac{q(t)}{C} \right) = 0 \\

\end{align}
$$
---

There is always 50% energy is wasted, like to resistors and wire.

([[07 - Capacitance#Energy Stored in Capacitors]])

$$
\begin{align}
U_{\text{source}}  & = Q_{\text{Max}} \cdot \epsilon = C \epsilon^2 \\
U_{\text{Capacitor}}  & = \frac{1}{2} Q_{f} \cdot \epsilon = \frac{1}{2} C \epsilon^2
\end{align}
$$

### Discharging the Capacitor

The negative sign in $i(t)$ in magnitude is that the current of capacitor when discharging is always sending current OUT.

$$
\begin{align}
-IR - \frac{q}{C}  & = 0 \\
q(t)  & = Q_{0} \cdot e^{- t/RC} \\
i(t)  & = - \frac{Q_{0}}{RC} e^{- t/RC} = i(0) \cdot e^{- t/RC}
\end{align}
$$

**Total Energy dissipated** is $$E = \frac{1}{2} C V_{0}^2$$  
**Energy dissipated as heat in the resistor:**

> The same as energy stored

$$
E = \frac{1}{2} C \mathcal{E}^2
$$

---

An interesting result is that exactly **half** of the total energy supplied by the source is dissipated as heat in the resistor, regardless of the value of R.
