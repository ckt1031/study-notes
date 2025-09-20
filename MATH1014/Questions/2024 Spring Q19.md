$$
f(x) = \sum_{n=0}^\infty (-1)^n \frac{(x-2)^{n+2}}{(n+1) \times 8^n}
$$

## Part A

Find the $\mathrm{4-th}$ order derivative $f^{''''} (2)$

---

$$
\begin{align}
f(x) &  = \sum_{k=0}^\infty \frac{f^{(k)}(a)}{k!} (x-a)^k \\
a  & =  2 \\
k  & = n + 2 \\
c_{k}  & = \frac{(-1)^{k-2}}{(k-1) \cdot 8^{k-2}}  \\
f^{(k)}(a)  & = k! \times c_k \\
 & = 4! \times \frac{1}{(4-1)\cdot 8^2} \\
 & = \frac{4 \times 3 \times 2}{3 \times 8 \times 8} \\
 & = \frac{1}{8}
\end{align}
$$

## Part B

Determine the interval of convergence of the power series.

---

$$
\begin{align}
L  & = \lim_{ n \to \infty } |\frac{a_{n+1}}{a_{n}}| \\
 & = \lim_{ n \to \infty } |\frac{(-1)^{n+1} (x-2)^{n+3}}{(n+2) \times 8^{(n+1)}} \frac{(n+1) \times 8^n}{(-1)^{n} (x-2)^{n+2}} |\\
 & = \lim_{ n \to \infty } |\frac{(-1) (x -2) ( n+1)}{8 (n+2)}| \\
 & = |x -2| \cdot\lim_{ n \to \infty } |\frac{( n+1)}{8 (n+2)}| \\
 & = \frac{|x-2|}{8}
\end{align}
$$

$$
-1 < \frac{x-2}{8} < 1 \Longleftrightarrow -8 < x - 2< 8 \Longleftrightarrow - 6 < x < 10
$$

For $x=-6$:

$$
\begin{align}
(-1)^n \frac{(-6)^{n+2}}{(n+1) \times 8^n}  & = (-1)^{2n} \frac{(8)^{n}}{(n+1) \times 8^n} \\
 & = \frac{1}{n+1} \\
 \frac{1}{n+1}  & \leq \frac{1}{n} \\
 \lim_{ n \to \infty } \frac{\frac{1}{n+1}}{\frac{1}{n}}  & = \lim_{ n \to \infty }  \frac{n}{n+1} = 1 \neq 0 < \infty
\end{align}
$$

Since harmonic series diverges, so $\sum^\infty_{0} \frac{1}{n+1}$ diverges when $x=-6$.

For $x=10$:

$$
\begin{align}
(-1)^n \frac{(8)^{n+2}}{(n+1) \times 8^n}  & = 64 \cdot(-1)^{n} \frac{1}{(n+1)} \\
\frac{d}{dx} \frac{1}{n+1}  & = - \frac{1}{(n+1)^2} < 0 \, (x \geq 0) \\
\lim_{ n \to \infty } \frac{1}{ n+1} & = 0
\end{align}
$$

By using alternating series test, the power series converges at $x=10$.

$$
\therefore (-6, 10]
$$

## Part C

Find the value of $f^{'}(4)$

---

$$
\begin{align}
f^{'}(x)  & = \sum_{n=0}^\infty (-1)^n \frac{(n+ 2) (x-2)^{n+1}}{(n+1) \times 8^n} \\
f^{'}(4)  & = \sum_{n=0}^\infty (-1)^n \frac{(n+ 2) (2)^{n+1}}{(n+1) \times 8^n} \\
	 & = 2 \sum_{n=0}^\infty (-1)^n \frac{n+ 2}{(n+1) \times 4^n} \\
	 & = 2 \sum_{n=0}^\infty (-1)^n \left( 1 + \frac{1}{n+1} \right) \frac{1}{4^n} \\
     & = 2 \sum_{n=0}^\infty \left[ \left( -\frac{1}{4} \right)^n + \frac{1}{n+1} \frac{1}{4^n} \right] \\
 & = 2 \frac{1}{1+\frac{1}{4}} + 2 \sum_{n=0}^\infty \frac{(-1)^n}{n+1} \frac{1}{4^n} \\
 & = \frac{8}{5} + 2 \cdot 4 \cdot \ln \left(  1+ \frac{1}{4} \right)
\end{align}
$$

Since $\ln(1+x) = \sum_{n=1}^\infty (-1)^{n-1} \frac{x^n}{n} = x - \frac{x^2}{2} + \frac{x^3}{3} - \frac{x^4}{4} + \cdots \quad \text{for } -1 < x \le 1$

And first value is $\frac{1}{4}$, but the series should be $1$ for first item.  
Second value is $-\frac{1}{2} \frac{1}{4^2}$, we want $-\frac{1}{2} \frac{1}{4}$, so whole $\ln (1+x) \times 4$
