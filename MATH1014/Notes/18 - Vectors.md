- Some physical quantities have both **magnitude** and **direction**; these are called **vector quantities**. Examples include velocity, force, momentum, and dipole moment. In contrast, scalar quantities like mass, charge, energy, and temperature are described by a single value.

## Distance Between Points

- Distance Formula (2D): The distance between $\left(x_{1}, y_{1}\right)$ and $\left(x_{2}, y_{2}\right)$ in the $xy$-plane is $\sqrt{\left(x_{2}-x_{1}\right)^{2}+\left(y_{2}-y_{1}\right)^{2}}$.
- Distance Formula (3D): The distance between $P_{1}\left(x_{1}, y_{1}, z_{1}\right)$ and $P_{2}\left(x_{2}, y_{2}, z_{2}\right)$ is $P_{1} P_{2}=\sqrt{\left(x_{1}-x_{2}\right)^{2}+\left(y_{1}-y_{2}\right)^{2}+\left(z_{1}-z_{2}\right)^{2}}$.  
- Example: The distance between $P_{1}(1,2,3)$ and $P_{2}(-1,1,2)$ is $\sqrt{(1-(-1))^{2}+(2-1)^{2}+(3-2)^{2}}=\sqrt{6}$.

## Spheres in Space

- Equation of a Sphere: A sphere with radius $r>0$ centered at $\left(x_{0}, y_{0}, z_{0}\right)$ is defined by the equation: $$(x-x_{0})^{2}+(y-y_{0})^{2}+(z-z_{0})^{2}=r^{2}$$
	- This means any point $(x,y,z)$ on the sphere is at a distance $r$ from the center.
- Example: The equation $x^{2}+y^{2}+z^{2}-2 x+4 y+1=0$ defines a sphere. By completing the square, it becomes $(x-1)^{2}+(y+2)^{2}+z^{2}=4=2^{2}$. This shows it is a sphere centered at $(1,-2,0)$ with radius 2.
- Inequalities and Regions:
	- $x^{2}+y^{2}+z^{2}-2 x+4 y+1 \leq 0$ (or $(x-1)^{2}+(y+2)^{2}+z^{2} \leq 2^{2}$) describes the points on and inside the sphere (a ball).
	- $x^{2}+y^{2}+z^{2}-2 x+4 y+1 \geq 0$ (or $(x-1)^{2}+(y+2)^{2}+z^{2} \geq 2^{2}$) describes the points on and outside the sphere.

## Using Coordinate Points As "Position Vectors"

> A coordinate point $P:(a, b)$ in the plane can define a position vector as an arrow from the origin $O$ to $P$.  
> This is sometimes denoted $\langle a, b\rangle$ to avoid confusion with coordinates. Similarly for 3D.

## Three Standard Unit Vectors

- The standard basic vectors are $\mathbf{i}=\langle 1,0,0\rangle$, $\mathbf{j}=\langle 0,1,0\rangle$, and $\mathbf{k}=\langle 0,0,1\rangle$. These are mutually perpendicular position vectors of length 1 pointing along the positive x, y, and z directions, respectively.  
- Any vector $\langle a, b, c\rangle$ can be written as a linear combination of these vectors: $\langle a, b, c\rangle=a \mathbf{i}+b \mathbf{j}+c \mathbf{k}$.  
- For forces, this decomposition means a force represented by $\langle 3,-2,5\rangle$ is the resultant force of three perpendicular components: $3 \mathbf{i}, -2 \mathbf{j}, 5 \mathbf{k}$.

## Unit Vectors

> A unit vector is a vector with length one.  

To find the unit vector in the same direction as a non-zero vector $\mathbf{v}$, divide the vector by its magnitude: $$\frac{\mathbf{v}}{|\mathbf{v}|}$$

- Example: The unit vector in the direction of $\langle 1,1,2\rangle$ is $\frac{1}{|\langle 1,1,2\rangle|}\langle 1,1,2\rangle=\frac{1}{\sqrt{6}}\langle 1,1,2\rangle=\left\langle\frac{1}{\sqrt{6}}, \frac{1}{\sqrt{6}}, \frac{2}{\sqrt{6}}\right\rangle$.

To find a vector in the same direction as $\mathbf{v}$ but with a magnitude $m$, multiply the unit vector by $m$: $m \frac{\mathbf{v}}{|\mathbf{v}|}$.

- Example: A vector in the same direction as $\langle 1,1,2\rangle$ with magnitude 6 is $6\left\langle\frac{1}{\sqrt{6}}, \frac{1}{\sqrt{6}}, \frac{2}{\sqrt{6}}\right\rangle=\langle\sqrt{6}, \sqrt{6}, 2 \sqrt{6}\rangle$.

> **Property**: $|c \mathbf{v}|=|c| \cdot|\mathbf{v}|$ for any real number $c$ and vector $\mathbf{v}$.

## Decomposing Vectors

- Any plane vector can be decomposed into the sum of components along two non-collinear directions using the parallelogram law.
- Similarly, any space vector can be decomposed into components along three non-coplanar directions.
- Decomposing a vector $\langle-1,5,8\rangle$ into components parallel to $\langle 1,0,1\rangle$, $\langle 1,1,2\rangle$, and $\langle 0,2,3\rangle$ means finding scalars $a, b, c$ such that $\langle-1,5,8\rangle=a\langle 1,0,1\rangle+b\langle 1,1,2\rangle+c\langle 0,2,3\rangle$. This involves solving a system of linear equations. The solution is $a=2, b=-3, c=4$.

## Directed Line Segments: Free Vectors

- Free vectors are geometric arrows not necessarily starting from the origin, from an initial point $A$ to a terminal point $B$, denoted $\overrightarrow{A B}$.
- **Triangle Law of Addition**: For position vectors $\overrightarrow{O A}=\mathbf{u}$ and $\overrightarrow{O B}=\mathbf{v}$, the position vector addition $\mathbf{u}+(\mathbf{v}-\mathbf{u})=\mathbf{v}$ corresponds to the free vector addition $\overrightarrow{O A}+\overrightarrow{A B}=\overrightarrow{O B}$.
- **Free Vector Subtraction**: $\overrightarrow{O B}-\overrightarrow{O A}=\overrightarrow{A B}$. This free vector $\overrightarrow{A B}$ is a parallel translate of the position vector $\mathbf{v}-\mathbf{u}$. Free vectors having the same length and direction are often considered the same vector (e.g., same force applied at different points).
- Any free vector $\overrightarrow{A B}$ is the parallel translate of a unique position vector starting from the origin.
- Addition/subtraction for free vectors **starting from a common point $C$** follow the triangle law: $\overrightarrow{C A}+\overrightarrow{A B}=\overrightarrow{C B}$ and $\overrightarrow{C B}-\overrightarrow{C A}=\overrightarrow{A B}$.

## Midpoint

> Midpoint Formula (3D): The midpoint $M$ of the line segment joining $P_{1}\left(x_{1}, y_{1}, z_{1}\right)$ and $P_{2}\left(x_{2}, y_{2}, z_{2}\right)$ is: $$\left(\frac{x_{1}+x_{2}}{2}, \frac{y_{1}+y_{2}}{2}, \frac{z_{1}+z_{2}}{2}\right)$$

This formula can be derived using vectors: $\overrightarrow{O M} = \overrightarrow{O P_{1}}+\frac{1}{2} \overrightarrow{P_{1} P_{2}}$.

## Dividing a Line Segment

For $0 < \lambda < 1$, the point $P$ dividing the segment $\overline{P_{1} P_{2}}$ such that $|P_{1}P|:|P_{1}P_{2}| = \lambda:1$ is given by $\overrightarrow{O P}=(1-\lambda) \overrightarrow{O P_{1}}+\lambda \overrightarrow{O P_{2}}$.

This formula also works for points on the extension of the segment if $\lambda<0$ or $\lambda>1$.

- Example: To find points dividing the segment from $(2,-3,5)$ to $(8,3,2)$ into three equal segments, use $\lambda=1/3$ and $\lambda=2/3$. The vector from $(2,-3,5)$ to $(8,3,2)$ is $\langle 8,3,2\rangle-\langle 2,-3,5\rangle=\langle 6,6,-3\rangle$.
	- For $\lambda=1/3$: $\langle 2,-3,5\rangle+\frac{1}{3}\langle 6,6,-3\rangle=\langle 4,-1,4\rangle$.  
	- For $\lambda=2/3$: $\langle 2,-3,5\rangle+\frac{2}{3}\langle 6,6,-3\rangle=\langle 6,1,3\rangle$.

```tikz
\begin{document}
\begin{tikzpicture}
    % Define the endpoints of the line segment
    % We use \coordinate to easily reference these points later
    \coordinate (A) at (0,0);
    \coordinate (B) at (5,0); % A horizontal segment of length 5

    % Define the dividing point P
    % Let's place P at (3,0). This divides the segment of length 5
    % into a segment AP of length 3 and a segment PB of length 2.
    % The ratio AP:PB is 3:2.
    \coordinate (P) at (3,0);

    % Draw the main line segment from A to B
    \draw (A) -- (B);

    % Draw small filled circles at the points to make them visible
    % Also add labels using nodes positioned below the points
    \fill (A) circle (2pt) node[below] {A};
    \fill (B) circle (2pt) node[below] {B};
    \fill (P) circle (2pt) node[below] {P};

    % Add annotations to show the two segments AP and PB
    % We use the decorations.pathreplacing library for braces
    % The 'mirror' option puts the brace below the path
    \draw (A) -- (P)
          node[below=7pt, midway] {AP}; % Text label below the brace

    \draw (P) -- (B)
          node[below=7pt, midway] {PB}; % Text label below the brace

    % Optional: Add a title or description above the diagram
    \node[above=5pt] at (current bounding box.north) {};
    \node[above=5pt] at (2.5,0) {AP:PB = 3:2}; % Show the ratio
\end{tikzpicture}
\end{document}
```

### Basic Properties of Vector Operations

| Law                                      | Property                                                                |
| ---------------------------------------- | ----------------------------------------------------------------------- |
| Commutative Law of Addition              | $\mathbf{u}+\mathbf{v}=\mathbf{v}+\mathbf{u}$                           |
| Associative Law of Addition              | $(\mathbf{u}+\mathbf{v})+\mathbf{w}=\mathbf{u}+(\mathbf{v}+\mathbf{w})$ |
| Identity Law of Addition                 | $\mathbf{u}+\overrightarrow{\mathbf{0}}=\mathbf{u}$                     |
| Inverse Law of Addition                  | $\mathbf{u}+(-\mathbf{u})=\overrightarrow{\mathbf{0}}$                  |
| ---                                      | $0 \mathbf{u}=\overrightarrow{\mathbf{0}}$                              |
| Identity Law of Scalar Multiplication    | $1 \mathbf{u}=\mathbf{u}$                                               |
| Associative Law of Scalar Multiplication | $a(b \mathbf{u})=(a b) \mathbf{u}$                                      |
| Distributive Law                         | $a(\mathbf{u}+\mathbf{v})=a \mathbf{u}+a \mathbf{v}$                    |
| Distributive Law                         | $(a+b) \mathbf{u}=a \mathbf{u}+b \mathbf{u}$                            |

### Angle Between Vectors (Dot Product)

- The angle $\theta$ between two non-zero vectors $\mathbf{u}$ and $\mathbf{v}$ can be found using the Cosine Law: $$|\mathbf{u}-\mathbf{v}|^{2}=|\mathbf{u}|^{2}+|\mathbf{v}|^{2}-2|\mathbf{u}||\mathbf{v}| \cos \theta$$
- Dot Product Definition: The dot product of two vectors $\mathbf{u}$ and $\mathbf{v}$ is defined as: $$\mathbf{u} \cdot \mathbf{v}=|\mathbf{u}||\mathbf{v}| \cos \theta$$
	- where $\theta$ is the angle between them.

Dot Product (Coordinate Form):

- In the plane: $\left\langle u_{1}, u_{2}\right\rangle \cdot\left\langle v_{1}, v_{2}\right\rangle=u_{1} v_{1}+u_{2} v_{2}$
- In space: $\left\langle u_{1}, u_{2}, u_{3}\right\rangle \cdot\left\langle v_{1}, v_{2}, v_{3}\right\rangle=u_{1} v_{1}+u_{2} v_{2}+u_{3} v_{3}$ (Derived from the Cosine Law)

**Finding the Angle**: From the definition, the angle can be found using: for non-zero $\mathbf{u}, \mathbf{v}$: $$\cos \theta=\frac{\mathbf{u} \cdot \mathbf{v}}{|\mathbf{u}||\mathbf{v}|}$$

- **Example**: The angle between $\langle 1,1,1\rangle$ and $\langle 0,0,1\rangle$ has $\cos \theta=\frac{\langle 1,1,1\rangle \cdot\langle 0,0,1\rangle}{|\langle 1,1,1\rangle||\langle 0,0,1\rangle|} = \frac{1}{\sqrt{3} \sqrt{1}}=\frac{1}{\sqrt{3}}$. So, $\theta=\cos ^{-1} \frac{1}{\sqrt{3}}$ radians.

## Basic Properties of Dot Product

- **Orthogonality**: Two non-zero vectors $\mathbf{u}$ and $\mathbf{v}$ are perpendicular (orthogonal) ==if and only if== $\mathbf{u} \cdot \mathbf{v}=0$. This implies $\theta=\frac{\pi}{2}$.  
- $\mathbf{u} \cdot \mathbf{u}=|\mathbf{u}|^{2} \geq 0$
- $|a \mathbf{u}|=|a||\mathbf{u}|$ (where $|a|$ is absolute value).  
- $\mathbf{u}=\overrightarrow{\mathbf{0}} \Longleftrightarrow|\mathbf{u}|=0$.  
- $\mathbf{u} \cdot \mathbf{v}=\mathbf{v} \cdot \mathbf{u}$ (Commutative Law of Dot Product).  
- $(a \mathbf{u}) \cdot \mathbf{v}=a(\mathbf{u} \cdot \mathbf{v})=\mathbf{u} \cdot(a \mathbf{v})$ (Associative Property w/ Scalar).  
- $\mathbf{u} \cdot(a \mathbf{v}+b \mathbf{w})=a \mathbf{u} \cdot \mathbf{v}+b \mathbf{u} \cdot \mathbf{w}$ (Distributive Law of Dot Product).

## Decomposing Vectors (using Dot Product)

- If $\mathbf{e}_1, \mathbf{e}_2, \mathbf{e}_3$ are three mutually perpendicular unit vectors in space, any vector $\mathbf{u}$ can be decomposed as: $$\mathbf{u}=\left(\mathbf{u} \cdot \mathbf{e}_{1}\right) \mathbf{e}_{1}+\left(\mathbf{u} \cdot \mathbf{e}_{2}\right) \mathbf{e}_{2}+\left(\mathbf{u} \cdot \mathbf{e}_{3}\right) \mathbf{e}_{3}$$  
- **Directional Cosines**: If a vector $\mathbf{u}$ makes angles $\alpha, \beta, \gamma$ with the positive x, y, z axes respectively, then the unit vector in the direction of $\mathbf{u}$ is $\frac{\mathbf{u}}{|\mathbf{u}|} = \langle\cos \alpha, \cos \beta, \cos \gamma\rangle$. These components $\cos \alpha, \cos \beta, \cos \gamma$ are called the directional cosines.
	- Note that $(\cos \alpha)^2 + (\cos \beta)^2 + (\cos \gamma)^2 = 1$.  
- *Example*: For $\mathbf{u}=\langle 1,2,-2\rangle$, the unit vector is $\frac{\mathbf{u}}{|\mathbf{u}|}=\left\langle\frac{1}{3}, \frac{2}{3},-\frac{2}{3}\right\rangle$. The angles with the axes are $\alpha=\cos ^{-1} \frac{1}{3}$, $\beta=\cos ^{-1} \frac{2}{3}$, $\gamma=\cos ^{-1} \frac{-2}{3}$.

## Work Done

- The work done ($W$) by a constant force $\overrightarrow{\mathbf{F}}$ causing a displacement $\overrightarrow{\mathbf{d}}$ is given by the dot product: $W=\overrightarrow{\mathbf{F}} \cdot \overrightarrow{\mathbf{d}}=|\overrightarrow{\mathbf{F}}||\overrightarrow{\mathbf{d}}| \cos \theta$, where $\theta$ is the angle between $\overrightarrow{\mathbf{F}}$ and $\overrightarrow{\mathbf{d}}$.  
- *Example*: If $|\mathbf{F}|=5 \mathrm{~N}$, $|\overrightarrow{\mathbf{d}}|=10 \mathrm{~m}$, and $\theta=\frac{\pi}{3}$, the work done is $W=5 \cdot 10 \cdot \cos \frac{\pi}{3}=25 \mathrm{~J}$.  
- Work done along a curve under a force field involves integrating the dot product ($\int_{C} \mathbf{F} \cdot d \mathbf{r}$), which is a sum of tiny work contributions.

## Orthogonal Projection (Vector Projection)

- **Vector Projection**: The orthogonal projection of vector $\mathbf{u}$ along vector $\mathbf{v} \neq \overrightarrow{\mathbf{0}}$ is a vector component of $\mathbf{u}$ that is parallel to $\mathbf{v}$. It is given by the formula: $$\text { Proj }_{\mathbf{v}} \mathbf{u}=\frac{\mathbf{u} \cdot \mathbf{v}}{|\mathbf{v}|^{2}} \mathbf{v}$$  
- **Scalar Projection**: The scalar projection (or scalar component) of $\mathbf{u}$ in the direction of $\mathbf{v}$ is the signed length of the vector projection. It is given by the formula: $\operatorname{comp}_{\mathbf{v}} \mathbf{u}=\frac{\mathbf{u} \cdot \mathbf{v}}{|\mathbf{v}|}$. This scalar is equal to $|\mathbf{u}| \cos \theta$.
- **Decomposition**: A vector $\mathbf{u}$ can be decomposed into two mutually perpendicular components: one parallel to $\mathbf{v}$ ($\text{Proj}_{\mathbf{v}} \mathbf{u}$) and one perpendicular to $\mathbf{v}$ ($\mathbf{u} - \text{Proj}_{\mathbf{v}} \mathbf{u}$).  
- *Example*: Decompose $\langle 3,2,2\rangle$ into components parallel and perpendicular to $\langle 1,1,1\rangle$.
	- Parallel component $\mathbf{p}$: $\text {Proj}_{\langle 1,1,1\rangle}\langle 3,2,2\rangle=\frac{\langle 3,2,2\rangle \cdot\langle 1,1,1\rangle}{1^{2}+1^{2}+1^{2}}\langle 1,1,1\rangle=\frac{7}{3}\langle 1,1,1\rangle=\left\langle\frac{7}{3}, \frac{7}{3}, \frac{7}{3}\right\rangle$.  
	- Perpendicular component $\mathbf{n}$: $\mathbf{n}=\langle 3,2,2\rangle-\mathbf{p}=\langle 3,2,2\rangle-\left\langle\frac{7}{3}, \frac{7}{3}, \frac{7}{3}\right\rangle=\left\langle\frac{2}{3}, -\frac{1}{3}, -\frac{1}{3}\right\rangle$. Note the calculation error in the source example for $\mathbf{n}$ coordinates.  
	- Pythagoras Theorem holds: $|\langle 3,2,2\rangle|^{2}=|\mathbf{p}|^{2}+|\mathbf{n}|^{2}$.

## Cross Product & Determinants (for 3D vectors)

- The cross product $\mathbf{u} \times \mathbf{v}$ is an operation that results in a vector perpendicular to both $\mathbf{u}$ and $\mathbf{v}$ (if they are not parallel).  
- Coordinate Formula: For $\mathbf{u}=\left\langle u_{1}, u_{2}, u_{3}\right\rangle$ and $\mathbf{v}=\left\langle v_{1}, v_{2}, v_{3}\right\rangle$, the cross product is: $$\mathbf{u} \times \mathbf{v}=\left\langle u_{2} v_{3}-u_{3} v_{2},-u_{1} v_{3}+u_{3} v_{1}, u_{1} v_{2}-u_{2} v_{1}\right\rangle$$  
- This can be written using **2x2 determinants**: $$\mathbf{u} \times \mathbf{v}=\left(\left|\begin{array}{cc} u_{2} & u_{3} \ v_{2} & v_{3} \end{array}\right|,-\left|\begin{array}{cc} u_{1} & u_{3} \ v_{1} & v_{3} \end{array}\right|,\left|\begin{array}{cc} u_{1} & u_{2} \ v_{1} & v_{2} \end{array}\right|\right)$$
- A $2 \times 2$ determinant is calculated as: $$\left|\begin{array}{ll}a & b \\ c & d\end{array}\right|=a d-b c$$
- Example: $\langle 1,2,-3\rangle \times\langle 2,4,1\rangle=\langle 14,-7,0\rangle$. Checking the dot product confirms it's perpendicular: $\langle 1,2,-3\rangle \cdot\langle 14,-7,0\rangle=0$ and $\langle 2,4,1\rangle \cdot\langle 14,-7,0\rangle=0$.  
- Standard Unit Vector Cross Products: $\mathbf{i} \times \mathbf{j}=\mathbf{k}, \quad \mathbf{j} \times \mathbf{k}=\mathbf{i}, \quad \mathbf{k} \times \mathbf{i}=\mathbf{j}$. The order matters: $\mathbf{j} \times \mathbf{i}=-\mathbf{k}, \quad \mathbf{k} \times \mathbf{j}=-\mathbf{i}, \quad \mathbf{i} \times \mathbf{k}=-\mathbf{j}$. Thus, $\mathbf{u} \times \mathbf{v} \neq \mathbf{v} \times \mathbf{u}$ in general.

## Some Properties of Cross Product

- $\mathbf{u} \times \mathbf{u}=\overrightarrow{\mathbf{0}}$.
- $\mathbf{u} \times \mathbf{v}=-\mathbf{v} \times \mathbf{u}$ (Anti-commutative).  
- $a(\mathbf{u} \times \mathbf{v})=(a \mathbf{u}) \times \mathbf{v}=\mathbf{u} \times(a \mathbf{v})$ (Associative Property w/ Scalar).  
- $\mathbf{u} \times(a \mathbf{v}+b \mathbf{w})=a \mathbf{u} \times \mathbf{v}+b \mathbf{u} \times \mathbf{w}$ (Distributive Law).

These properties can be used for computation, e.g., $(2 \mathbf{i}-3 \mathbf{k}) \times(3 \mathbf{i}+2 \mathbf{j}-\mathbf{k}) = 6 \mathbf{i}-7 \mathbf{j}+4 \mathbf{k}$. This matches the coordinate calculation $\langle 2,0,-3\rangle \times\langle 3,2,-1\rangle=\langle 6,-7,4\rangle$.

## Geometric Properties of the Cross Product

- **Direction**: The direction of $\mathbf{u} \times \mathbf{v}$ is perpendicular to both $\mathbf{u}$ and $\mathbf{v}$. The vectors $\mathbf{u}$, $\mathbf{v}$, and $\mathbf{u} \times \mathbf{v}$ in that order follow the right-hand rule.
- **Length (Magnitude)**: If $\theta$ is the angle between $\mathbf{u}$ and $\mathbf{v}$, the magnitude of the cross product is: $$|\mathbf{u} \times \mathbf{v}|=|\mathbf{u}||\mathbf{v}| \sin \theta$$
- **Area of Parallelogram**: The magnitude $|\mathbf{u} \times \mathbf{v}|$ equals the area of the parallelogram generated by $\mathbf{u}$ and $\mathbf{v}$.

## Area of a Triangle

- The area of a triangle with vertices P, Q, R is half the area of the parallelogram formed by the vectors $\overrightarrow{PQ}$ and $\overrightarrow{PR}$ (or any pair of vectors representing two sides originating from the same vertex).
- Area of triangle: $$\frac{1}{2} |\overrightarrow{PQ} \times \overrightarrow{PR}|$$  
- Example: For vertices $(1,-1,0)$, $(2,1,-1)$, and $(-1,1,2)$, the vectors from $(1,-1,0)$ are $\mathbf{u}=\langle 1,2,-1\rangle$ and $\mathbf{v}=\langle-2,2,2\rangle$. The cross product is $\langle 1,2,-1\rangle \times\langle-2,2,2\rangle=\langle 6,0,6\rangle$. The area of the triangle is $\frac{1}{2} |\langle 6,0,6\rangle|=\frac{1}{2} \sqrt{6^2+0^2+6^2} = \frac{1}{2}\sqrt{72} = 3\sqrt{2}$.

## Volume of A Parallelepiped (Scalar Triple Product)

- The volume of the parallelepiped generated by three vectors $\mathbf{u}, \mathbf{v}, \mathbf{w}$ is given by the magnitude of the scalar triple product: Volume is: $$|\mathbf{w} \cdot(\mathbf{u} \times \mathbf{v})|$$
- Geometrically, $|\mathbf{u} \times \mathbf{v}|$ is the area of the base parallelogram, and $|\mathbf{w} \cdot \frac{\mathbf{u} \times \mathbf{v}}{|\mathbf{u} \times \mathbf{v}|}|$ is the height (the scalar projection of $\mathbf{w}$ onto the vector normal to the base).

## Finding a Vector Perpendicular to a Plane

- To find a vector perpendicular to the plane containing three points, first form two vectors that lie in the plane by connecting one point to the other two. The cross product of these two vectors will be perpendicular to the plane.
- Example: For the plane through $(1,-1,0)$, $(2,1,-1)$, and $(-1,1,2)$, two vectors in the plane are $\langle 1,2,-1\rangle$ and $\langle-2,2,2\rangle$. Their cross product $\langle 1,2,-1\rangle \times\langle-2,2,2\rangle=\langle 6,0,6\rangle$ is perpendicular to the plane.  
- To find unit vectors perpendicular to the plane, normalize the resulting vector: $\pm \frac{1}{|\langle 6,0,6\rangle|}\langle 6,0,6\rangle= \pm\left\langle\frac{1}{\sqrt{2}}, 0, \frac{1}{\sqrt{2}}\right\rangle$.

## 3x3 Determinant / Triple Scalar Product

$$\left|\begin{array}{lll}a_{1} & a_{2} & a_{3} \\ b_{1} & b_{2} & b_{3} \\ c_{1} & c_{2} & c_{3}\end{array}\right|=a_{1}\left|\begin{array}{cc}b_{2} & b_{3} \\ c_{2} & c_{3}\end{array}\right|-a_{2}\left|\begin{array}{cc}b_{1} & b_{3} \\ c_{1} & c_{3}\end{array}\right|+a_{3}\left|\begin{array}{cc}b_{1} & b_{2} \\ c_{1} & c_{2}\end{array}\right|$$

- The 3x3 determinant with row vectors $\mathbf{a}, \mathbf{b}, \mathbf{c}$ is equal to the scalar triple product $\mathbf{a} \cdot(\mathbf{b} \times \mathbf{c})$.  
- Its *absolute* value is the **volume of the parallelepiped** generated by $\mathbf{a}, \mathbf{b}, \mathbf{c}$.  
- **Coplanar Vectors**: Three vectors are lying on the same plane if and only if their associated determinant (scalar triple product) is zero.  
- *Example*: The volume of the parallelepiped generated by $(1,2,-1),(1,0,1),(2,3,0)$ is the absolute value of the determinant formed by these vectors. Let's use the order $\mathbf{u}=(1,2,-1), \mathbf{v}=(1,0,1), \mathbf{w}=(2,3,0)$. The source calculates the determinant of a matrix formed by vectors $(1,0,1), (2,3,0), (1,2,-1)$ yielding $-2$. The volume is $|-2|=2$.  
- The volume of the tetrahedron generated by these vectors is $\frac{1}{6}$ of the volume of the parallelepiped, i.e., $\frac{1}{6} \cdot 2=\frac{1}{3}$.

## Cross Product in Physics

- Torque ($\tau$): For a force $\mathbf{F}$ acting at a point with position vector $\mathbf{r}$ relative to the pivot, the torque is $\tau = \mathbf{r} \times \mathbf{F}$.  
- Lorentz Force: The force acting on a moving charge $q$ with velocity $\mathbf{v}$ in a magnetic field $\mathbf{B}$ is $\mathbf{F} = q(\mathbf{v} \times \mathbf{B})$.
