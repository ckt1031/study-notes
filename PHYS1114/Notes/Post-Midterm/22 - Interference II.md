***Assume light strikes the surface at normal incidence (perpendicularly).***

## Thin-Film Interference

<img src="https://obsidian-img-studies.tsun1031.xyz/2025/08/01/d99d36dabc607715c833fe302bff69f4.png" height="250px" />

> When light shines on two glass plates separated by a thin wedge of air, interference patterns (fringes) appear.
>
> This is due to the interaction between light waves reflecting from the bottom surface of the top plate and the top surface of the bottom plate.

A crucial concept is the **phase change upon reflection**. A 180° (or half-cycle) phase shift occurs when light traveling in a medium reflects off the surface of a medium with a higher refractive index.

- For $n_{a} > n_{b}$, no phase change. (glass-to-air)
- For $n_{a} = n_{b}$, no reflection.  
- For $n_{a} < n_{b}$, **half cycle phase change**. (air-to-glass)

Since there is one of two reflected rays with half phase change, ==the conditions of interference is inverted.==

$$
x = \left( \frac{l}{h} \right) t =m \frac{l\lambda_{0}}{2h}
$$

- $l$ is **total horizontal length of the air wedge**.
- $x$ **represents the horizontal distance**.
- $\lambda_{0}$ **wavelength of light in a vacuum**.

### Constructive Interference

$$
\begin{align}
\Delta \phi_{\text{total}}  & = \Delta \phi_{\text{path}} + \Delta \phi_{\text{ref}} \\
\Delta \phi_{\text{path}}  & = \frac{2\pi}{\lambda} \Delta r = \frac{4\pi t}{\lambda} \\
2m \pi & = \Delta \phi_{\text{tot}} = \frac{4\pi t}{\lambda} + \pi \\
2t  & =\left( m+\frac{1}{2} \right) \lambda
\end{align}
$$

## Destructive Interference

$$
\begin{align}
\Delta \phi_{\text{tot}}  & = 2m\pi+\pi \\
2t  & = m\lambda
\end{align}
$$

## Point of contact in an Air Wedge

![image](https://obsidian-img-studies.tsun1031.xyz/2025/08/01/83cd2e0c17c042cc847c941d9297c732.png)

At the point of contact, the path difference $2t$ is zero.

However, the light ray reflecting from the bottom glass plate (air-to-glass boundary) undergoes a 180° phase shift, while the ray reflecting from the top plate (glass-to-air) does not. This **inherent phase difference of half a cycle** causes destructive interference, resulting in a dark fringe.

## No or Both Half Phase Change

If no or both has phase change, ==their conditions are also **swapped**, i.e. $2t = m \lambda$ for constructive interference and $2t = \left(m+\frac{1}{2} \right) \lambda$ for destructive interference,==

![image](https://obsidian-img-studies.tsun1031.xyz/2025/07/30/62b7936be2403ddf887e3f55dd99c3e8.png)  

**For a thin film of plastic in air (Air-Plastic-Air):**

- The first reflection is at the **air-to-plastic** surface. Since $n_{air​}<n_{plastic}$​, a **phase change occurs**.
- The first reflection is at the **plastic-to-air** surface. Since $n_{air​}<n_{plastic}$​, **no phase change occurs**.

> Only one phase change.

**For a thin film of silicone between plastic and flint glass (Plastic-Silicone-Flint Glass):**

- The first reflection is at the **plastic-to-silicone** surface. Since plastic (n=1.40) has a lower refractive index than silicone (n=1.50), a **phase change occurs**.
- The second reflection is at the silicone-to-flint glass surface. Since silicone (n=1.50) has a lower refractive index than flint glass (n=1.60), a phase change also occurs here.

### Conditions

Depends on the **net phase difference** and what we want, i.e. we want more reflection or want more destruction.

$\Delta\Phi_{ref}$ is the difference in phase change between the reflection of Ray 1 (at the top interface) and the reflection of Ray 2 (at the bottom interface).

1. **Ray 1:** This is the light ray that reflects off the **top surface** of the film.
2. **Ray 2:** This is the light ray that **enters the film**, reflects off the **bottom surface** of the film, and then exits the film to interfere with Ray 1.

#### $\Delta\Phi_{ref} = 0$

> or $2\pi$, i.e., both or neither reflection has a $\pi$ phase change

- **Constructive Reflection**: $2 n_{film} t = m \lambda_{vacuum}$ ($m=1, 2, 3…$ for non-zero thickness)  
- **Destructive Reflection**: $2 n_{film} t = (m + 1/2) \lambda_{vacuum}$ ($m=0, 1, 2…$)

#### $\Delta\Phi_{ref} = \pi$

> i.e., one reflection has a $\pi$ phase change and the other does not

- **Constructive Reflection**: $2 n_{film} t = (m + 1/2) \lambda_{vacuum}$ ($m=0, 1, 2…$)  
- **Destructive Reflection**: $2 n_{film} t = m \lambda_{vacuum}$ ($m=1, 2, 3…$ for non-zero thickness)

### Vertical Bubble

If a soap bubble is held vertically, why do colored horizontal bands appear, and why do they seem to move downwards over time?

![image](https://obsidian-img-studies.tsun1031.xyz/2025/08/01/6ac5ae8816b97ec59547a6f69a531342.png)

**The horizontal bands are areas of uniform thickness**, where constructive interference occurs for a specific color (wavelength).

As gravity continues to pull the water down, **the entire film gets thinner, causing the bands of a specific thickness (and color) to move downwards.**

- **Front Surface (Air-to-Water):** Reflection occurs off a medium with a higher refractive index, causing a **180° phase shift**.
- **Back Surface (Water-to-Air):** Reflection occurs off a medium with a lower refractive index, causing **no phase shift**.

Because there is one net phase shift, the condition for **constructive interference** (bright colors)

Thicker at bottom, larger $t$, larger $m$.

## Application of Interference

### Newton's Ring

When a convex lens is placed on a flat glass plate, a thin air wedge with circular symmetry is formed. The resulting circular interference fringes are known as **Newton's rings**.

This phenomenon is used to test the ==precision of lenses==, any imperfections in the lens's curvature will show up as irregularities in the fringe pattern.

### Thin vs. Thick Films

Interference effects are only visible in **thin films (thickness of a few micrometers).**

This is because light from common sources is emitted in short, incoherent bursts. In a thin film, rays reflected from the top and bottom surfaces originate from the same burst and are thus  **coherent**, allowing them to interfere. 

In a **thick film**, the reflected rays come from different bursts, are ==not coherent==, and therefore do not produce a stable interference pattern.

### Non-Reflective Coatings

For a non-reflective coating, we want **reflected rays to interfere destructively.**

Only the range below can apply quick formula, if not, we have to use: $\Delta \phi$

$$
n_{\text{glass}} > n_{\text{film}} > n_{\text{air}}
$$

> Ensures that both reflections (air-to-film and film-to-glass) cause a $\pi$ phase shift.

**Thickness:**

$$
\begin{align}
2t  & = \left( m + \frac{1}{2} \right) \lambda \\
 2t  & = \frac{\lambda}{2} \\
 t  & = \boxed{\frac{\lambda}{4}} \\
 & = \frac{\lambda_{0}}{4 n _{\text{film}}}
\end{align}
$$

> This causes destructive interference for reflected light, which in turn **increases the amount of transmitted light.**

> For eye glasses, 550 nm is **yellowish green** where the eye is most sensitive.

#### Still Have Some Reflective Color?

Assume a non-reflective coating designed for **550 nm (green) light**. (maximum destructive interference)

It is less effective for wavelengths at the ends of the visible spectrum, such as blue and red light. Therefore, these colors **are more strongly reflected**. The combination of reflected red and blue light appears purplish to the eye.

### The Michelson Interferometer

![image](https://obsidian-img-studies.tsun1031.xyz/2025/07/30/5b988fb703e59331be1aa7a1c3b05f91.png)

1. A beam of monochromatic light from a source is split by a **beam splitter**, a partially silvered mirror.
2. One ray travels to a **fixed** mirror (M2​) and the other to a movable mirror (M1).
3. A **compensator plate** (C) is placed in the path of the ray going to M2 to ensure both rays travel through the same thickness of glass.
4. The rays reflect off their respective mirrors, recombine at the beam splitter, and travel to an observer, creating an interference pattern.

By moving the mirror M1​ a distance of $λ/2$, the total path length of that arm (**path that light travels between the beam splitter and a mirror**) ==changes== by $λ$. This causes the entire interference pattern to shift by one full fringe.

The movement of the mirror is **parallel** to the light ray traveling along that arm, towards or backwards the ray.
