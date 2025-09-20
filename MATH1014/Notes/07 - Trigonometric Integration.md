## Trigonometric Integration

* $\sqrt{a^2 - x^2}$: $x = a \sin \theta$
* $\sqrt{a^2 + x^2}$: $x = a \tan \theta$
* $\sqrt{x^2 - a^2}$: $x = a \sec \theta$

$$
\begin{align*}
\int \sec(x) \, dx &= \ln|\sec(x) + \tan(x)| + C \\
&= \ln\left|\tan\left(\frac{x}{2} + \frac{\pi}{4}\right)\right| + C \\
&= \operatorname{arcsinh}(\tan x) + C
\end{align*}
$$

$$
\begin{align*}
\int \tan(x) \, dx &= \ln|\sec(x)| + C \\
&= -\ln|\cos(x)| + C
\end{align*}
$$

## Arc Trigonometry

$$
\begin{align}  
\frac{\mathrm{d}}{\mathrm{d}x} \arcsin x & = \frac{1}{\sqrt{ 1 - x^2 }} \\  
\frac{\mathrm{d}}{\mathrm{d}x} \arctan x & = \frac{1}{1+ x^2} \\  
\frac{\mathrm{d}}{\mathrm{d}x} \arccos x & = \frac{-1}{\sqrt{ 1 - x^2 }}  
\end{align}
$$

$$\begin{align}
\int \frac{1}{u^2 + a^2} du & = \frac{1}{a} \arctan\left(\frac{u}{a}\right) + C \\
\int \frac{1}{\sqrt{a^2 - x^2}} dx &= \arcsin\left(\frac{x}{a}\right) + C \\
\int \frac{-1}{\sqrt{a^2 - x^2}} dx &= \arccos\left(\frac{x}{a}\right) + C
\end{align}$$

### Example of Using Arc Trigonometry

$$
\begin{align}  
\int{\frac{x+2}{x^2+x+1}} & = \int \frac{\frac{1}{2} (2x+1) + \frac{3}{2}}{x^2+x+1} dx \\  
& = \frac{1}{2} \int \frac{2x+1}{x^2+x+1} dx + \frac{3}{2} \int \frac{1}{x^2+x+1} dx \\  
& = \frac{1}{2} \ln(x^2+x+1) + \frac{3}{2} \int \frac{1}{(x+\frac{1}{2})^2 + \frac{3}{4}} dx \\  
& = \frac{1}{2} \ln(x^2+x+1) + \frac{3}{2} \cdot \frac{2}{\sqrt{3}} \arctan\left(\frac{x+\frac{1}{2}}{\frac{\sqrt{3}}{2}}\right) + C \\  
& = \frac{1}{2} \ln(x^2+x+1) + \sqrt{3} \arctan\left(\frac{2x+1}{\sqrt{3}}\right) + C  
\end{align}
$$


## Wallis's Integral Formula

$$
\int_0^{\pi/2} \sin^n x \, dx = \int_0^{\pi/2} \cos^n x \, dx =  
\begin{cases}  
	\frac{(n-1)(n-3)\cdots 1}{n(n-2)\cdots 2} \cdot \frac{\pi}{2} & \text{if } n \text{ is even} \\  
	\frac{(n-1)(n-3)\cdots 2}{n(n-2)\cdots 3} & \text{if } n \text{ is odd}  
\end{cases}
$$

## Sine Reduction Formula

$$
\begin{align}  
\int \sin^n x \, dx & = -\frac{1}{n} \sin^{n-1} x \cos x + \frac{n-1}{n} \int \sin^{n-2} x \, dx \\  
\int \cos^n x \, dx & = + \frac{1}{n} \cos^{n-1} x \sin x + \frac{n-1}{n} \int \cos^{n-2} x \, dx  
\end{align}
$$

## Tangent Reduction Formula

$$
\begin{align}  
\int \tan^n x \, dx & = \frac{1}{n-1} \tan^{n-1} x - \int \tan^{n-2} x \, dx \\  
\int \sec^n x \, dx & = \frac{\sec^{n-2}x \tan x}{n-1} + \frac{n-2}{n-1}\int \sec^{n-2} x \, dx  
\end{align}
$$

$$
\frac{1}{64} \cdot 6 \cdot 9.8 \cdot 1000 =
$$
