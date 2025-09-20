An L-R-C series circuit is constructed using a $175 \ \Omega$ resistor, a $12.5 \ \mu \text{F}$ capacitor, and an $8.00 \ \text{mH}$ inductor, all connected across an ac source having a variable frequency and a voltage amplitude of $25.0 \ \text{V}$.

## Part A

At what angular frequency will the impedance be smallest?

---

$$
\begin{align}
\omega = \frac{1}{ \sqrt{ 8 \times 10^{-3} \times 12.5 \times 10^{-6} }} \approx 3160 \ \mathrm{rad/s}
\end{align}
$$

## Part B

What is the impedance at this frequency?

---

At the resonance frequency, **the total impedance Z is equal to the resistance**.

> $\min Z = \min \sqrt{ R^2 + \left(\omega  L- \frac{1}{\omega C} \right)^2 } = \sqrt{ R^2 } = R$

$$
Z = R
$$

## Part C

At the angular frequency in part A, what is the maximum current through the inductor?

$$
I_{max} = \frac{V_{max}}{Z} = \frac{25}{175}= 0.143 \ \mathrm{A}
$$

## Part D

At the angular frequency in part A, find the potential difference across the ac source, the resistor, the capacitor, and the inductor at the instant that the current is equal to one-half its greatest positive value.

---

$$
\begin{align}
i  & = I \cos (\omega t) \\
 & = \frac{I}{2} \\
wt  & = \frac{\pi}{3} \\
V_{R}  & = I R \frac{1}{2} \\
 & = 12.5 \ \mathrm{V} \\
V_{L}  & = I \omega L \cos\left( \frac{\pi}{3} + \frac{\pi}{2} \right) \\
 & = -3.13 \ \mathrm{ V} \\
V_{C}  & =  \frac{I}{\omega C} \cos \left( \omega t - \frac{\pi}{2} \right) \\
 & = 3.13 \ \mathrm{V}
\end{align}
$$
