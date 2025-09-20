## Integration by Parts

This technique is the integral counterpart of the product rule for differentiation. Recall the product rule:

$$
\frac{d}{d x}[u(x) v(x)]=u(x) v^{\prime}(x)+v(x) u^{\prime}(x)
$$

Rearranging and integrating both sides, we obtain the integration by parts formula:

$$
\int u(x) v^{\prime}(x) d x=u(x) v(x)-\int v(x) u^{\prime}(x) d x
$$

Or, using differential notation ($du = u'(x)dx$, $dv = v'(x)dx$):

$$
\int u \, dv=u v-\int v \, du
$$

**Key Idea:** Integration by parts transforms one integral ($\int u \, dv$) into another ($\int v \, du$). The goal is to choose `u` and `dv` such that the new integral is easier to solve than the original.

**Tips for Choosing `u` and `dv`:**

* Often, you want `u` to be a function that simplifies when differentiated (e.g., `x`, `ln x`, `arctan x`).
* `dv` should be something you can readily integrate.
* Sometimes, it is not obvious which function to assign as u or v, do some trial and error can help

## LIATE Rule

| Category              | Function Type              | Example                 | Why it's a Good Choice for *u*                                                        |
| --------------------- | -------------------------- | ----------------------- | ------------------------------------------------------------------------------------- |
| Logarithmic           | $\ln(x)$, $\log_2(x)$      | $\int \ln(x) \, dx$     | Derivative simplifies to $\frac{1}{x}$.                                               |
| Inverse Trigonometric | $\arctan(x)$, $\arcsin(x)$ | $\int \arctan(x) \, dx$ | Derivative is algebraic and often simplifies.                                         |
| Algebraic             | $x^2$, $3x+1$, $\sqrt{x}$  | $\int x \sin(x) \, dx$  | Derivative reduces the power of $x$.                                                  |
| Trigonometric         | $\sin(x)$, $\cos(x)$       | $\int x \cos(x) \, dx$  | Integral and derivative cycle between sine and cosine.  Sometimes works well as *dv*. |
| Exponential           | $e^x$, $2^x$               | $\int x e^x \, dx$      | Integral remains exponential.  Often works well as *dv*.                              |

## Partial Fraction Decomposition

This technique is used to integrate rational functions (ratios of polynomials).

**Key Idea:** Any rational function `p(x)/q(x)` can be expressed as a sum of simpler fractions, called partial fractions, provided the degree of `p(x)` is less than the degree of `q(x)` (if not, perform polynomial long division first). These simpler fractions are easier to integrate.

**General Form of Partial Fractions:**

After factoring the denominator `q(x)` completely, the partial fraction decomposition will involve terms of the following forms:

* For each linear factor `(x - a)` to the power `k`:

	$$
    \frac{A_1}{x - a} + \frac{A_2}{(x - a)^2} + \dots + \frac{A_k}{(x - a)^k}
    $$

* For each irreducible quadratic factor `(x - a)^2 + b^2` to the power `k`:

	$$
    \frac{A_1x + B_1}{(x - a)^2 + b^2} + \frac{A_2x + B_2}{((x - a)^2 + b^2)^2} + \dots + \frac{A_kx + B_k}{((x - a)^2 + b^2)^k}
    $$
	Which can be further broken down into:
	$$
\frac{A(x-a)}{\left((x-a)^{2}+b^{2}\right)^{k}}+\frac{B+A a}{\left((x-a)^{2}+b^{2}\right)^{k}}
$$

**Example:** (Conceptual - full decomposition is not shown)

Suppose you want to integrate  `(x + 1) / (x(x - 1)^2)`.  The partial fraction decomposition would look like this:

$$
\frac{x + 1}{x(x - 1)^2} = \frac{A}{x} + \frac{B}{x - 1} + \frac{C}{(x - 1)^2}
$$

You would then solve for the constants  `A`,  `B`, and  `C`, and integrate each term separately. The resulting integrals are typically logarithms and/or powers of  `(x - a)`.

## Hyperbolic Functions

*   **Hyperbolic Sine:** $\sinh(x) = \frac{e^x - e^{-x}}{2}$
*   **Hyperbolic Cosine: $\cosh(x) = \frac{e^x + e^{-x}}{2}$
*   **Hyperbolic Tangent:** $\tanh(x) = \frac{e^x - e^{-x}}{e^x + e^{-x}}$
*   $\sinh(ix) = i\sin x$
*   $\cosh(ix) = \cos x$
*   $\sin(ix) = i\sinh x$
*   $\cos(ix) = \cosh x$

### For Integrals of the Form $\sqrt{x^2 \pm a^2}$ or $\sqrt{a^2 - x^2}$

This technique is especially useful for dealing with integrals containing square roots.

*   **For $\sqrt{x^2 + a^2}$:**  Let $x = a\sinh t$, then $dx = a\cosh t \, dt$ and $\sqrt{x^2 + a^2} = a\cosh t$.
*   **For $\sqrt{x^2 - a^2}$:**  Let $x = a\cosh t$, then $dx = a\sinh t \, dt$ and $\sqrt{x^2 - a^2} = a\sinh t$, where $x > a$.
*   **For $\sqrt{a^2 - x^2}$:**  Let $x = a\tanh t$, then $dx = a\text{sech}^2 t \, dt$ and $\sqrt{a^2 - x^2} = a\text{sech }t$, where $|x| < a$.

### Special Cases and Tricks

*   **Integrals involving powers of $\sinh x$ and $\cosh x$:** Use identities to reduce the powers, often converting to expressions involving $\sinh(nx)$ or $\cosh(nx)$.
*   **Integrals involving $\tanh x$ or $\coth x$:** Rewrite these in terms of $\sinh x$ and $\cosh x$, and then use u-substitution or other techniques.
*   **Integrals of the form $\int \frac{1}{a + b\cosh x} \, dx$ or $\int \frac{1}{a + b\sinh x} \, dx$:** These can often be solved by using the exponential definitions of $\sinh x$ and $\cosh x$ and then using a suitable substitution.
