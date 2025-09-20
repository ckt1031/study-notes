Iterate the recurrence to derive that the solution to:

$$
T(n) = \begin{cases}  
   3 T\left( \frac{n}{3} \right) + n & \text{if } n \ge 3 \\  
   1 & \text{if } n < 3  
\end{cases}
$$

---

$$\begin{align}
T(n) &= 3 \times T\left(\frac{n}{3} \right) + 3 \\
T(n) &= 3 \times \left(3 T\left(\frac{n}{3^2} \right) + \frac{n}{3} \right) + n \\
T(n) &= 3^2 \times T\left(\frac{n}{3^2} \right) + 2n \\
T(n) &= 3^3 \times T\left(\frac{n}{3^3} \right) + 3n \\
T(n) &= 3^i \times T\left(\frac{n}{3^i} \right) + in \\
\text{We have }i &= \log_{3} n \\
 & = 3^{\log_{3} n} \times T\left(\frac{n}{3^{\log_{3} n}} \right) + (\log_{3} n) \cdot n \\
\end{align}
$$

Solution is $\Theta (n \log n)$.
