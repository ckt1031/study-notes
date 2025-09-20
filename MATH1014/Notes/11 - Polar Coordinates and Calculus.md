## Common Shapes

### Circle

$$
\begin{align}
\text{Green}  &  = a \sin \theta \\
\text{Red}  &  = a \cos \theta
\end{align}
$$

![image](https://obsidian-img-studies.tsun1031.xyz/2025/05/18/6b47c87ffaadc5ac81e8e9270cf277a3.png)

### Limacons (Snails)

- Equation: $r = a \pm b \cos \theta$ or $r = a \pm b \sin \theta$ (where $a > 0$ and $b > 0$)

#### Cardioid (Heart-shaped): $a = b$

The curve passes through the origin and has a cusp there.  
Example: $r = 1 + \cos \theta$, $r = 2 - 2 \sin \theta$.

![image](https://obsidian-img-studies.tsun1031.xyz/2025/05/18/f1098f178faaa393f9af72b7924552d3.png)

#### Dimpled Limacon: $a > b$

The curve does not pass through the origin and has a "dent" but no inner loop.  
Example: $r = 3 + \cos \theta$, $r = 2 - \sin \theta$.

![image](https://obsidian-img-studies.tsun1031.xyz/2025/05/18/20cf10d593ff8912bd1bd5703f19f77e.png)

#### Limacon with an Inner Loop: $a < b$

The curve has both an outer loop and an inner loop. The inner loop is traced when $r$ is negative.  
Example: $r = 1 + 2 \cos \theta$, $r = 1 - 2 \sin \theta$. (As discussed in the previous example)

![image](https://obsidian-img-studies.tsun1031.xyz/2025/05/18/21e4389880976acec3f6a05c4d84fcf4.png)

#### Convex Limacon: $a \ge 2b$ (sometimes Included with Dimpled limacons)

The curve is convex and does not have a dent or inner loop.  
Example: $r = 3 + \cos \theta$ (also a dimpled limacon), $r = 4 - \sin \theta$.

![image](https://obsidian-img-studies.tsun1031.xyz/2025/05/18/f22c8763273403438b0bd4e6f59dcae0.png)

### Rose Curves

> Equation: $r = a \cos(n\theta)$ or $r = a \sin(n\theta)$ (where $a \ne 0$ and $n$ is a positive integer)  

- If n is odd: The curve has $n$ petals.  
- If n is even: The curve has $2n$ petals.
- For $n$ is odd, if petals aligns with $x$-axis, it is a cosine rose. Otherwise, it is a sine rose.
- For $n$ is even, if petals cut with $x$-axis and $y$-axis, it is a cosine rose. Otherwise, it is a sine rose.

$$
r=3\cos(2\theta) \quad r=3\sin(5\theta)
$$

![image](https://obsidian-img-studies.tsun1031.xyz/2025/05/18/0c6c2880b59ee5e317f8fe831f8d7fda.png)

### Spirals

Equation: $r = a\theta$ or $r^2 = a\theta$ (where $a$ is a non-zero constant)

Description: Curves that spiral outward from or inward towards the origin as $\theta$ increases or decreases.

#### Archimedean Spiral: $r = a\theta$

The distance between successive turns of the spiral is constant.

Example: $r = \theta$ (for $\theta \ge 0$).

For $a> 0$, the spiral moves in the counterclockwise direction.

#### Fermat's Spiral: $r^2 = a\theta$

Example: $r^2 = \theta$ (for $\theta \ge 0$).

### Lemniscates

> Figure-eight shaped curves.  
> Equation: $r^2 = a^2 \cos(2\theta)$ or $r^2 = a^2 \sin(2\theta)$ (where $a \ne 0$)

- $r^2 = a^2 \cos(2\theta)$: Symmetric about the x-axis.  
- $r^2 = a^2 \sin(2\theta)$: Symmetric about the line $y=x$.

## Polar Coordinates (r, θ)

- **Definition:** A point in the xy-plane can be represented by polar coordinates (r, θ), where:
	- **Radial Coordinate (r):** The distance of the point from the origin (the distance from (x,y) to (0,0)).
	- **Angular Coordinate (θ):** The angle formed by the line segment connecting the origin to the point and the positive x-axis, measured counterclockwise.
- **Non-Uniqueness of θ:** The angular coordinate θ is ==not unique==. The points (r, θ) and (r, θ + 2kπ), where k is any integer, represent the same point.

### Conversion between Polar and Rectangular Coordinates

- From $(r, \theta)$ to $(x, y)$:
	- $x = r \cos \theta$
	- $y = r \sin \theta$
- From $(x, y)$ to $(r, \theta)$:
	- $r^2 = x^2 + y^2$ (or $r = \sqrt{x^2 + y^2}$)
	- $\tan \theta = y/x$ (Careful with quadrants when finding $\theta$)

## Symmetry of Polar Curves

- **Symmetry about the x-axis:** If replacing $\theta$ with -$\theta$ in the equation results in an equivalent equation (F(r, -$\theta$) = F(r, $\theta$)), the curve is symmetric about the x-axis.
- **Symmetry about the y-axis:** If replacing $\theta$ with $\pi$ - $\theta$ in the equation results in an equivalent equation (F(r, $\theta$) = F(r, $\pi$ - $\theta$)), the curve is symmetric about the y-axis.
- **Symmetry about the origin:** If either of the following conditions is met, the curve is symmetric about the origin:
	- Replacing r with -r results in an equivalent equation (F(-r, $\theta$) = F(r, $\theta$)).
	- Replacing $\theta$ with $\pi$ + $\theta$ results in an equivalent equation (F(r, $\theta$) = F(r, $\pi$ + $\theta$)).

## Slope of a Tangent Line

- For a curve defined by $r = r(\theta)$, the slope of the tangent line at a given point can be found using the chain rule:
	- $\frac{dy}{dx} = \frac{dy/d\theta}{dx/d\theta}$
- Recall the conversion formulas and their derivatives with respect to $\theta$:
	- $x = r(\theta) \cos \theta \implies \frac{dx}{d\theta} = r'(\theta) \cos \theta - r(\theta) \sin \theta$
	- $y = r(\theta) \sin \theta \implies \frac{dy}{d\theta} = r'(\theta) \sin \theta + r(\theta) \cos \theta$

Therefore, the slope of the tangent line is:

$$\frac{dy}{dx} = \frac{r'(\theta) \sin \theta + r(\theta) \cos \theta}{r'(\theta) \cos \theta - r(\theta) \sin \theta}$$

## Area in Polar Coordinates

- The area of a region bounded by the rays $\theta = a$ and $\theta = b$ and the polar curve $r = r(\theta)$ is given by the integral: $$A = \frac{1}{2} \int_{a}^{b} [r(\theta)]^2 \ \mathrm{d}\theta$$
- This formula is derived by summing the areas of tiny sectors (like pizza slices) with angle $\Delta\theta$ and radius $r(\theta)$, where the area of each sector is approximately $\frac{1}{2} \cdot r^2\Delta\theta$.

## Arc Length in Polar Coordinates

- The arc length $L$ of a polar curve $r = r(\theta)$ from $\theta = a$ to $\theta = b$ is given by the integral: $$L = \int_{a}^{b} \sqrt{r^{2} + (\frac{dr}{d\theta})^{2}} \ d\theta$$
- This formula is derived from approximating the curve with small line segments. The square of the length of a tiny segment is approximately $(\Delta x)^{2} + (\Delta y)^{2}$.
- Using $\frac{dx}{d\theta}$ and $\frac{dy}{d\theta}$, we get: $$(\frac{dx}{d\theta})^{2} + (\frac{dy}{d\theta})^{2} = r^{2} + (\frac{dr}{d\theta})^{2}$$

## Inner Loop and Outer Loop

The inner loop occurs when $r$ is negative. This means that the point is located in the opposite direction of the angle $\theta$.

- **Example**: $1+ 2 \sin \theta$, since $r = 1 + 2 \sin \theta$, the inner loop is traced when $1 + 2 \sin \theta < 0$, which means $\sin \theta < -1/2$. This occurs for $\theta$ in the interval $(7\pi/6, 11\pi/6)$.
