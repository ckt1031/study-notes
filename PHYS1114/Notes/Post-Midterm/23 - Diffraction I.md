When light encounters an obstacle or an aperture, it doesn't simply cast a sharp shadow as geometric optics would predict.

Instead, the light bends around the edges of the obstacle. This phenomenon is known as **diffraction**.

> In experiments with non-laser light, coherence is typically achieved by using a single source and splitting the light (e.g., with a double slit).

## Single-Slit Fraunhofer Diffraction

### Huygens's Principle

Every point on a wavefront can be considered a source of secondary spherical wavelets.

The new wavefront is the superposition of all these wavelets. For a single slit, we imagine the opening is divided into many infinitesimally small, parallel strips, each acting as a source of ==Huygens's wavelets.==

Source ↔ slit ↔ screen are all _effectively at infinity_ → outgoing rays to the screen are **parallel**.

### Finding the Dark Fringes (Minima)

If the path difference between these two wavelets **is half a wavelength**, they will cancel out each other.

A $\lambda/2$ path difference means the two waves reach the screen **$180^\circ$ out of phase** and their electric fields cancel.

**First Minimum ($m=\pm1$)**:

Consider dividing the slit of width 'a' into _two halves_. If we pair a wavelet from the very top edge of the slit with a wavelet from the center, ==these two will interfere destructively== at a certain angle $\theta$ if their path difference is half a wavelength ($\lambda/2$). This condition is given by:

$$
\frac{a}{2} \sin \theta = \frac{\lambda}{2} \implies a \sin \theta = \lambda
$$

When this condition is met,  _every_ wavelet from the upper half of the slit destructively interferes with a corresponding wavelet from the lower half, resulting in **zero intensity (a dark fringe)** at that angle.

**Other Minima ($m=±2, ±3, …$)**:

For the second minimum, we divide the slit into four equal parts. The path difference between the top edge and the bottom edge will be $2\lambda$. This ensures that the top quarter cancels with the second quarter, and the third quarter cancels with the fourth, again resulting in a ==minimum==.

$$a \sin \theta = k \lambda$$  

> $m=0$ is excluded because there is no path difference $a$.

Therefore, the entire slit produces a dark fringe at this angle.

### Intensity in the Single-Slit Pattern

The intensity of the light at any point on the screen is not uniform. The central fringe is the brightest and widest, with subsequent bright fringes becoming progressively dimmer.

To determine the intensity at any point in the pattern, we must **sum the contributions of all wavelets**. This can be done using a ==phasor diagram==.

$$
\begin{align}  
\beta & = ka \sin \theta = \frac{2\pi}{\lambda} a \sin \theta  
\end{align}
$$

$$
\begin{align}  
E_{P} & = E_{0} \frac{\sin\left(\beta / 2 \right)}{\beta / 2} \\  
I & = I_{0} \left[\frac{\sin\left(\beta / 2 \right)}{\beta / 2} \right]^2 \quad (\text{Use radian mode}) 
\end{align}
$$

- **Minima are exact**
- Maxima are ==approximate==, cannot be solved using simple algebra.

### Central Maximum

The angular width of the central maximum is the **angle between the first dark fringes on either side.**

$$
2 \theta_{1} = 2 \sin^{-1} \left(\frac{\lambda}{a} \right)
$$

The central bright fringe is **twice as wide as the other bright fringes**.

For small angles, this can be ==approximated== as:

$$
\text{Angular width} \approx \frac{2 \lambda}{a}
$$

When $m = \beta =0$ (all wavelets in phase), intensity is maximum due to $$\lim_{ x \to 0 } \frac{\sin x}{x} =1$$

### Secondary Maxima

The smaller bright fringes occur approximately halfway between the dark fringes. Their intensity falls off rapidly.

$$
I_{m} \approx \frac{I_{0}}{\left(m + \frac{1}{2} \right)^2 \pi ^2} \quad (I_{1} \approx 4.5\%, I_{2} \approx 1.6\%, I_{3} \approx0.83\%)
$$

### Intensity Minimum

Intensity is zero when $\sin \frac{\beta}{2} =0$, for $m$ is non-zero integer:

$$\begin{align}
\frac{\beta}{2}  & = \frac{\pi}{\lambda} a \sin \theta =m \pi \\
\theta  & = \sin^{-1} \left( \frac{m \lambda}{a} \right)
\end{align}$$

### Slit Width and Pattern

The width of the diffraction pattern is inversely proportional to the width of the slit 'a'.

A  **narrower slit** produces a **wider** diffraction pattern. Conversely, a wider slit produces a narrower, sharper central peak.

### No Minima Condition

If the slit width 'a' is less than or equal to the wavelength $\lambda$ ($a \leq \lambda$), the first minimum cannot form because $\sin\theta$ would have to be greater than 1.

In this case, ==the diffraction pattern is just one broad central maximum.==

## Double-Slit Interference


The classic Young's double-slit experiment produces a pattern of equally spaced bright and dark fringes.

The simple model assumes the slits are infinitesimally narrow, predicting that all bright fringes have the same intensity.

In reality, each slit has a finite width 'a'. Therefore, the observed pattern is a combination of two effects:

- **A double-slit interference pattern**, governed by the distance 'd' between the centers of the slits.
- **A single-slit diffraction pattern**, governed by the width 'a' of each slit.


![image](https://obsidian-img-studies.tsun1031.xyz/2025/08/01/29b2f1dd28bd06e6f2374702f98eafbf.png)

$$\boxed{\frac{a}{d} = \frac{k}{m}}$$

$$
\begin{align}  
I & = I_{0} \times (\text{Diffraction}) \times(\text{Interference}) \\  
 & = I_{0} \left[\frac{\sin (\beta / 2)}{\beta / 2} \right]^2 \cos^2 \left(\frac{\phi}{2} \right)  
\end{align}
$$

> For an ideal double-slit pattern (assuming infinitely narrow slits), both the minima and the maxima are located at ==precise, predictable positions.==


Dark fringe: $d\sin\theta=(m+\frac{1}{2})\lambda$

### Missing Maxima

Sometimes, a bright fringe predicted by the double-slit interference formula ($d \sin\theta = m_{i} \lambda$) coincides with a dark fringe from the single-slit diffraction envelope ($a \sin\theta = m_{d} \lambda$).

When this happens, **that particular bright fringe will be missing from the pattern.**

$$\frac{d}{a} = \frac{N+1}{2}$$

> The number of **interference** fringes ($N$) observed in the central diffraction maximum

A maximum is missing if both conditions are met for the **same angle θ**.

$$
\begin{align}  
\frac{d \sin \theta}{a \sin \theta} & = \frac{m_{i} \lambda}{m_{d} \lambda} \\  
\frac{d}{a} & = \frac{m_{i}}{m_{d}}  
\end{align}
$$

**Question**: If two slits of width `a` are separated by a distance `d = 2.5a`, are there any missing maxima?

$$
\frac{5}{2} = \frac{m_{i}}{m_{d}}
$$

$$(m_{i}, m_{d}) \in \{(5,2), (10, 4), \dots\}$$

## Concepts

- $d$ (distance between centers of slits) $\rightarrow$ **INTERFERENCE**
- $a$ (width of a single slit) $\rightarrow$ **DIFFRACTION**


|                            | Maxima (Bright)                                    | Minima (Dark)                             |
| -------------------------- | -------------------------------------------------- | ----------------------------------------- |
| Double-Slit (Interference) | $d \sin \theta = m \lambda$                        | $d \sin \theta = (m+\frac{1}{2}) \lambda$ |
| Single-Slit (Diffraction)  | $a\sin \theta=\left( m+\frac{1}{2}\right) \lambda$ | $a \sin \theta = m \lambda$               |
| Diffration grating         | $d \sin \theta = m\lambda$                         |                                           |

**Interference is the superposition of a few, distinct waves, while diffraction is the bending and spreading of a single wave as it encounters an obstacle or opening.**
