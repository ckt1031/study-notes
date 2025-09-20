> Tutorial Problem.

A $17.0 \ \mu \text{F}$ capacitor is charged by a $125.0 \ \text{V}$ power supply, then disconnected from the power and connected in series with a $0.280 \ \text{mH}$ inductor.

## Part A

Calculate the oscillation frequency of the circuit.

$$
\begin{align}
\omega &  = \frac{1}{\sqrt{ LC }} = \frac{1}{\sqrt{ 0.280 \times 10^{-3} \times 17 \times 10^{-6} }} \\
f  & = \frac{\omega}{2\pi} = 2.3 \ \mathrm{KHz}
\end{align}
$$

## Part B

Calculate the energy stored in the capacitor at time $t=0 \ \mathrm{ms}$ (the moment of connection with the inductor).

$$
\begin{align}
\frac{1}{2} CV^2 = 0.133 \ \mathrm{J}
\end{align}
$$

## Part C

Calculate the energy stored in the inductor at $t = 1.30 \ \mathrm{ms}$.

$$
\begin{align}
q(t)  & = Q \cos(\omega t + \phi) \\
i(t) & = \frac{dq}{dt} = - Q \omega \sin ( \omega t) \\
 & = - CV \omega \sin (\omega t) \\
U(t)  & = \frac{1}{2} L (CV \omega \sin (\omega t))^2  \\
 & = \frac{1}{2} (0.280 \times 10^{-3}) (17 \times 10^{-6}\times 125 \times 14494 \sin(14494 \times 1.30 \times 10^{-3}))^2 \\
 & = 6.5 \times 10^{-6} \ \mathrm{J}
\end{align}
$$
