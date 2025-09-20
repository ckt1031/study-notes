## Partial Fraction Decomposition

### Case 1: Distinct Linear Factors

If $q(x)$ can be factored into distinct linear factors, i.e., $q(x) = (x-a_1)(x-a_2)…(x-a_n)$, then the partial fraction decomposition takes the form:

$$\frac{p(x)}{q(x)} = \frac{A_1}{x-a_1} + \frac{A_2}{x-a_2} + \cdots + \frac{A_n}{x-a_n}$$

where $A_1, A_2, …, A_n$ are constants to be determined.

**Example:** $\frac{1}{(x-1)(x+2)} = \frac{A}{x-1} + \frac{B}{x+2}$

### Case 2: Repeated Linear Factors

If $q(x)$ has a repeated linear factor, i.e., $q(x) = (x-a)^k q_1(x)$, where $(x-a)$ is not a factor of $q_1(x)$, then the decomposition includes terms for each power of the repeated factor:

$$\frac{p(x)}{q(x)} = \frac{A_1}{x-a} + \frac{A_2}{(x-a)^2} + \cdots + \frac{A_k}{(x-a)^k} + \frac{p_1(x)}{q_1(x)}$$

where $A_1, A_2, …, A_k$ are constants to be determined, and $\frac{p_1(x)}{q_1(x)}$ is the remaining part of the decomposition.

**Example:** $\frac{1}{(x-1)^2(x+2)} = \frac{A}{x-1} + \frac{B}{(x-1)^2} + \frac{C}{x+2}$

### Case 3: Irreducible Quadratic Factors

If $q(x)$ has an irreducible quadratic factor (a quadratic that cannot be factored into linear factors with real coefficients), i.e., $q(x) = [(x-a)^2 + b^2]^k q_1(x)$, where $(x-a)^2 + b^2$ is not a factor of $q_1(x)$, then the decomposition includes terms of the form:

$$\frac{p(x)}{q(x)} = \frac{B_1x + C_1}{(x-a)^2 + b^2} + \frac{B_2x + C_2}{[(x-a)^2 + b^2]^2} + \cdots + \frac{B_kx + C_k}{[(x-a)^2 + b^2]^k} + \frac{p_1(x)}{q_1(x)}$$

where $B_1, …, B_k, C_1, …, C_k$ are constants to be determined, and $\frac{p_1(x)}{q_1(x)}$ is the remaining part of the decomposition.

**Example:** $\frac{1}{(x^2+1)(x+2)} = \frac{Ax+B}{x^2+1} + \frac{C}{x+2}$
