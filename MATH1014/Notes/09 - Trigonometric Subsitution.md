$$
\cos ^{2} x+\sin ^{2} x=1
$$
$$
1+\tan ^{2} x=\sec ^{2} x
$$

## Integrating Products

| Integral Form                   | Condition     | Substitution   | Identity Used                                                          |
|:------------------------------ |:------------ |:------------- |:--------------------------------------------------------------------- |
| $\int \sin^n(kx) \cos^m(kx) dx$ | *n* odd       | $u = \cos(kx)$ | $\sin^2(kx) = 1 - \cos^2(kx)$                                          |
| $\int \sin^n(kx) \cos^m(kx) dx$ | *m* odd       | $u = \sin(kx)$ | $\cos^2(kx) = 1 - \sin^2(kx)$                                          |
| $\int \sin(ax)\cos(bx)dx$, etc. |               | N/A            | Product-to-Sum Formulas                                                |
| $\int \sin^n(kx) \cos^m(kx) dx$ | *n*, *m* even | N/A            | $\sin^2(x) = \frac{1-\cos(2x)}{2}$, $\cos^2(x) = \frac{1+\cos(2x)}{2}$ |
| ---                             |               |                |                                                                        |
| $\int \tan^n(kx) \sec^m(kx) dx$ | *m* even      | $u = \tan(kx)$ | $\sec^2(kx) = 1 + \tan^2(kx)$                                          |
| $\int \tan^n(kx) \sec^m(kx) dx$ | *n* odd       | $u = \sec(kx)$ | $\tan^2(kx) = \sec^2(kx) - 1$                                          |

* If both n and m are even in $\int \tan^n(kx)\sec^m(kx)dx$, we can still use $u=tan(kx)$.
