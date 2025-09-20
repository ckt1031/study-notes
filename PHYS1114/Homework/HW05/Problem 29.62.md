A bar with mass $M = 1.20 \ \mathrm{kg}$ and resistance $R = 0.500 \ \Omega$ slides without friction on a horizontal U-shaped rail with width $W = 40.0 \ \mathrm{cm}$ and negligible resistance. The bar is attached to a spring with spring constant $k = 90.0 \ \mathrm{N/m}$, as shown in (Figure 1). A constant magnetic field with magnitude $1.00 \ \mathrm{T}$ points into the plane everywhere in the vicinity. At time $t = 0$ the bar is stretched beyond its equilibrium position by an amount $x = 10.0 \ \mathrm{cm}$ and released from rest.

![image](https://obsidian-img-studies.tsun1031.xyz/2025/07/16/ed59728efa573d040019b69b8feb40bd.png)

$$
\begin{align}
F_{Spring} + F_{Magnetic Damping}  & = Ma  \\
-kx - \frac{B^2W^2}{R} \frac{dx}{dt}  & = M \frac{d^2x}{dt^2}
\end{align}
$$

## Part A

This system behaves like a damped oscillator. What is the damping coefficient $b$?

$$
\begin{align}
\varepsilon  & = BWv \\
I  & = \frac{\varepsilon}{R} = \frac{BWv}{R} \\
F_{m}  & =IWB = \left( \frac{BWv}{R} \right) WB
 \\
 & = \frac{B^2W^2v}{R} \\
 & = \boxed{\frac{B^2W^2}{R}} \frac{dx}{dt}
\end{align}
$$

## Part B

With what frequency does the bar oscillate around its equilibrium position?

> Damped angular frequency

$$
\begin{align}
\omega_{0}  & = \sqrt{ \frac{k}{M} } \\
\gamma  & =\frac{b}{2M} \\
w^{'}  & =  \\
f  & = \frac{1}{2\pi} \sqrt{ \frac{k}{M} - \frac{b^2}{4M^2} }
\end{align}
$$

## Part C

What is the amplitude of the motion at time $t = 5.00 \ \mathrm{s}$

$$
x (t)  = \boxed{A_{0} e^{-\gamma t}} \cos(w^{'} t+\phi)
$$
