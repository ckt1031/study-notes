## Taylor and Maclaurin Series

A power series representation of a function $f(x)$ centered at $a$ has the form:  
$$f(x) = \sum_{k=0}^\infty c_k (x-a)^k = c_0 + c_1(x-a) + c_2(x-a)^2 + c_3(x-a)^3 + \dots$$

### Taylor Series

If a function $f(x)$ has a power series representation centered at $a$, that representation is its Taylor series at $a$. The coefficients of the Taylor series are directly related to the derivatives of $f$ at $a$:

$$f(x) = \sum_{n=0}^{\infty} \frac{f^{(n)}(a)}{n!} (x-a)^n = f(a) + f'(a)(x-a) + \frac{f''(a)}{2!}(x-a)^2 + \frac{f'''(a)}{3!}(x-a)^3 + \cdots + \frac{f^{(n)}(a)}{n!}(x-a)^n + \cdots$$

By comparing the coefficients of $(x-a)^k$ in the general power series form and the Taylor series form, we have:  
$$c_k = \frac{f^{(k)}(a)}{k!}$$

### Maclaurin Series

This is a special case of the Taylor series where the center is $a=0$.

$$f(x) = \sum_{n=0}^{\infty} \frac{f^{(n)}(0)}{n!} x^n = f(0) + f'(0)x + \frac{f''(0)}{2!}x^2 + \frac{f'''(0)}{3!}x^3 + \cdots + \frac{f^{(n)}(0)}{n!}x^n + \cdots$$

If a function has a power series representation centered at $0$:

$$f(x) = \sum_{k=0}^\infty c_k x^k = c_0 + c_1 x + c_2 x^2 + c_3 x^3 + \dots$$  
Then, by comparing coefficients:  
$$c_k = \frac{f^{(k)}(0)}{k!}$$

## Taylor's Theorem with Remainder

$$f(x) = \sum_{k=0}^{n} \frac{f^{(k)}(a)}{k!} (x-a)^k + R_n(x)$$  
- where $R_n(x) = \int_{a}^{x} \frac{(x-t)^{n}}{n!} f^{(n+1)}(t) dt$.
- $f(x) = \sum_{n=0}^{\infty} \frac{f^{(n)}(a)}{n!} (x-a)^n$ if and only if $\lim_{n \rightarrow \infty} R_n(x) = 0$.

$$R_n(x) = \frac{f^{(n+1)}(c)}{(n+1)!}(x-a)^{n+1}$$

## Common Maclaurin Series

- **Exponential Function:** $$ e^x = \sum_{n=0}^\infty \frac{x^n}{n!} = 1 + x + \frac{x^2}{2!} + \frac{x^3}{3!} + \cdots \quad \text{for all } x \in \mathbb{R} $$
- **Sine Function:** $$ \sin(x) = \sum_{n=0}^\infty (-1)^n \frac{x^{2n+1}}{(2n+1)!} = x - \frac{x^3}{3!} + \frac{x^5}{5!} - \frac{x^7}{7!} + \cdots \quad \text{for all } x \in \mathbb{R} $$
- **Cosine Function:** $$ \cos(x) = \sum_{n=0}^\infty (-1)^n \frac{x^{2n}}{(2n)!} = 1 - \frac{x^2}{2!} + \frac{x^4}{4!} - \frac{x^6}{6!} + \cdots \quad \text{for all } x \in \mathbb{R} $$
- **Natural Logarithm:** $$ \ln(1+x) = \sum_{n=1}^\infty (-1)^{n-1} \frac{x^n}{n} = x - \frac{x^2}{2} + \frac{x^3}{3} - \frac{x^4}{4} + \cdots \quad \text{for } -1 < x \le 1 $$
- **Arctangent Function:** $$ \arctan(x) = \sum_{n=0}^\infty (-1)^n \frac{x^{2n+1}}{2n+1} = x - \frac{x^3}{3} + \frac{x^5}{5} - \frac{x^7}{7} + \cdots \quad \text{for } |x| \le 1 $$

### Extra Notes of Maclaurin Series

- $\frac{1}{1-x} = \sum_{n=0}^{\infty} x^n = 1 + x + x^2 + \cdots$ for $|x| < 1$.
- $\frac{1}{1+x} = \sum_{n=0}^{\infty} (-1)^n x^n = 1 - x + x^2 - \cdots$ for $|x| < 1$.
- $\frac{1}{1+x^2} = \sum_{n=0}^{\infty} (-1)^n x^{2n} = 1 - x^2 + x^4 - \cdots$ for $|x| < 1$.
- $\frac{1}{(1-x)^2} = \sum_{n=0}^{\infty} (n+1) x^n = 1 + 2x + 3x^2 + \cdots$ for $|x| < 1$.
