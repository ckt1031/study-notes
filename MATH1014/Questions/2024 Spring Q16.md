Use the Maclaurin polynomial of $xe^{\cos \frac{x}{5}}$ of degree $3$ (i.e., Taylor polynomial of degree $3$ centered at $a=0$) to find an approximate value of the integral $\int_{0}^{1} 200xe^{\cos \frac{x}{5}}dx$.

---

$$
\begin{align}
\cos\left( \frac{x}{5} \right)  & = 1 - \frac{\left( \frac{x}{5} \right)^2}{2!} + \dots \\
e^{\cos \frac{x}{5}}  & = e^{\left( 1 - \frac{\left( \frac{x}{5} \right)^2}{2!} + \dots \right)} = e \cdot e^{\frac{\left( \frac{x}{5} \right)^2}{2!} + \dots}  \\
& = e \left[  1 + \left( - \frac{\left( \frac{x}{5} \right)^2}{2!} + \dots \right)+\frac{\left( - \frac{\left( \frac{x}{5} \right)^2}{2!} + \dots \right)^2}{2} + \dots  \right] \\
x\cos\left( \frac{x}{5} \right)  & = ex - \frac{x^3e}{50} \\
200 \int_{0}^{1} xe^{\cos \frac{x}{5}}dx  & = 200\int^{1}_{0} ex - \frac{x^3e}{50} \, dx \\
 & = 200 \left[ \frac{ex^2}{2} - \frac{x^4}{4} \frac{e}{50} \right]^1_{0} \\
 & = 200 \left( \frac{e}{2} - \frac{e}{200} \right) \\
 & = 100e - 1e = 99e
\end{align}
$$
