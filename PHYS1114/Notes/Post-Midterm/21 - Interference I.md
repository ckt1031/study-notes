$$
\lambda_{n} n = \lambda_{\text{vaccum}}
$$

## Fundamentals of Interference

### Coherence and Superposition

Interference happens when two or more waves overlap in the same region of space.

The resulting effect is by the **principle of superposition**, which states that the total wave amplitude at any point is ==the vector sum of the individual wave amplitudes at that point.==

For interference to **be observable with light**, the sources must be **coherent**.

> They must emit light of a ==single frequency (monochromatic)== and maintain a ==constant phase relationship== with each other.

### Constructive Interference

Occurs when two waves are **in phase** (their crests and troughs align perfectly).

Their amplitudes add up, resulting in a wave with a larger amplitude.

$$
\Delta l = m \lambda
$$

### Destructive Interference

This occurs when two waves are $\pi \ \text{radians}$ ($180^\circ$) out of phase (the crests of one wave align with the troughs of the other).

Their amplitudes **cancel each other out**, resulting in a wave with a smaller or even zero amplitude.

$$
\Delta l = \left( m+\frac{1}{2} \right) \lambda
$$

## Young's Double-Slit Experiment

Monochromatic light passes through a single slit and then through two parallel slits, $S_{1}$ and $S_{2}$, which are separated by a distance $d$.

These two slits act as **coherent sources**, creating an interference pattern of bright and dark bands (fringes) on a distant screen.

$$
\text{Path difference} = d \sin \theta
$$

For ==small angles==, we can use the approximation:

$$
\begin{align}
\sin \theta \approx \tan \theta  & \approx \frac{y}{L} \\
y_{m}  & =\frac{m\lambda L}{d}
\end{align}
$$

### Phase Difference

$k$ is the wave number.

$$
\phi = k (r_{2} - r_{1})= \frac{2\pi}{\lambda} (r_{2} - r_{1})
$$

For very far away from screen, their path $r_{1}$ and $r_{2}$ are **nearly parallel**:

$$
r_{2} - r_{1} =d \sin \theta
$$

## Intensity Distribution

$$
I \propto E^2
$$

**For two interfering waves:**

$E_{p}$ is resultant amplitude, $E$ is amplitude of each individual wave.

$$
E_{p} = 2 E \left| \cos \left( \frac{\phi}{2} \right) \right|
$$

Intensity at any point in the interference pattern:

$$
I = I_{0} \cos^2 \left(  \frac{\phi}{2} \right)
$$

$I_{0}$ is ==four times== the intensity of a single source, not double, because interference redistributes the energy.

By substituting the phase difference $\phi = k (d \sin \theta)$:

$$
I = I_{0} \cos^2 \left( \frac{2\pi}{\lambda} \frac{d\sin \theta}{2} \right) = I_{0} \cos^2 \left( \frac{\pi d\sin \theta}{\lambda} \right) 
$$

Using the **SMALL angle approximation**:

$$
I = I_{0} \cos^2 \left(  \frac{\pi dy}{\lambda L} \right)
$$
