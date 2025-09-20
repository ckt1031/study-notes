## Tips

* **Symmetry:** If the region is symmetric, you can often integrate over half the region and multiply the result by 2.

## Area Between Curves

$$
\text{Area (Bounded with x-axis)} = \int_a^b [f(x) - g(x)] \, dx
$$

```tikz
\usepackage{tikz}
\begin{document}
\begin{tikzpicture}[scale=1.5]
  % Axes
  \draw[->] (-0.5,0) -- (4.5,0) node[right] {$x$};
  \draw[->] (0,-0.5) -- (0,4.5) node[above] {$y$};

  % Curves
  \draw[thick,blue] plot[smooth] coordinates {(0.5,3) (1,2.5) (2,2.8) (3,3.5)};
  \node[blue] at (3.5,3.6) {$y=f(x)$};
  \draw[thick,red] plot[smooth] coordinates {(0.5,1) (1,1.2) (2,1.8) (3,2)};
  \node[red] at (3.5,2.1) {$y=g(x)$};

  % Area shading
  \fill[orange!30] (0.5,1) -- plot[smooth] coordinates {(0.5,3) (1,2.5) (2,2.8) (3,3.5)} --
    plot[smooth] coordinates {(3,2) (2,1.8) (1,1.2) (0.5,1)} -- cycle;

  % Labels for bounds
  \draw[dashed] (0.5,-0.2) -- (0.5,4);
  \node at (0.5,-0.4) {$a$};
  \draw[dashed] (3,-0.2) -- (3,4);
  \node at (3,-0.4) {$b$};
  
\end{tikzpicture}


\end{document}
```

$$\text{Area (Bounded with y-axis)} = \int_c^d [h(y) - k(y)] \, dy$$

```tikz
\usepackage{tikz}
\begin{document}
\begin{tikzpicture}[scale=1.5]
  % Axes (swapped x and y)
  \draw[->] (0,-0.5) -- (0,4.5) node[above] {$x$};  % x-axis now vertical
  \draw[->] (-0.5,0) -- (4.5,0) node[right] {$y$};  % y-axis now horizontal

  % Curves (coordinates swapped and labels rotated)
  \draw[thick,blue] plot[smooth] coordinates {(3,0.5) (2.5,1) (2.8,2) (3.5,3)};
  \node[blue] at (3.6,3.5) {$x=h(y)$}; % Label rotated
  \draw[thick,red] plot[smooth] coordinates {(1,0.5) (1.2,1) (1.8,2) (2,3)};
  \node[red] at (2.1,3.5) {$x=k(y)$}; % Label rotated

  % Area shading (coordinates swapped)
  \fill[orange!30] (1,0.5) -- plot[smooth] coordinates {(3,0.5) (2.5,1) (2.8,2) (3.5,3)} --
      plot[smooth] coordinates {(2,3) (1.8,2) (1.2,1) (1,0.5)} -- cycle;

  % Labels for bounds (positions adjusted)
  \draw[dashed] (-0.2,0.5) -- (4,0.5);
  \node at (-0.4,0.5) {$d$};
  \draw[dashed] (-0.2,3) -- (4,3);
  \node at (-0.4,3) {$c$};

\end{tikzpicture}
\end{document}
```

## Riemann Sum Approximation

The definite integral formula arises from the limit of a Riemann sum. Consider dividing the interval $[a, b]$ into $n$ subintervals of equal width $\Delta x = \frac{b-a}{n}$. Let $x_i$ be the right endpoint of the $i$-th subinterval. Then the Riemann sum approximating the area between the curves $y = f(x)$ and $y = g(x)$ is:

$$
A \approx \sum_{i=1}^{n} [f(x_i) - g(x_i)] \Delta x
$$

Taking the limit as $n \rightarrow \infty$, we obtain the definite integral:

$$
A = \lim_{n \rightarrow \infty} \sum_{i=1}^{n} [f(x_i) - g(x_i)] \Delta x = \int_{a}^{b} [f(x) - g(x)] dx
$$

## Example

Find the value(s) of such that the area of the region bounded by the parabolae $y=x^2-c^2$ and $y=c^2-x^2$ is $72$.

---

$$
\begin{align}
x^2 - c^2  & = c^2 - x^2  \\
x  & = \pm c \\
\int^c_{-c} 2x^2 - 2c^2 dx  & = \left[ \frac{2}{3} x^3 - 2c^2 x \right]^c_{-c} \\
 & = \frac{4}{3} c^3 - 4 c^3 \\
 & = - \frac{8}{3} c^3 \\
A  & = \frac{8}{3} c^3 \\
c & = \pm 3
\end{align}
$$
