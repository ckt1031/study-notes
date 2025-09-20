## Recursively Defined Function

### Arithmetic Sequence

$$a_{\text{n}} = a_{\text{n-1}} + d$$
- $d$: common difference

## Recurrence

### Solving First-Order Linear Recurrence

Solve the following recurrence:  
$f(0) = a$  
$f(n) = bf(n-1) + c$ for $n > 0$  
where $a$, $b$, $c$ are constants.

#### Solution

$f(n) = bf(n-1) + c$  
$= b(bf(n-2) + c) + c$  
$= b^2f(n-2) + bc + c$  
$= b^2(bf(n-3) + c) + bc + c$  
$= b^3f(n-3) + b^2c + bc + c$  
$\vdots$  
$= b^nf(0) + b^{n-1}c + b^{n-2}c + \dots + c$  
$= ab^n + c(b^{n-1} + b^{n-2} + \dots + 1)$  
$= ab^n + c \cdot \frac{b^{n}-1}{b-1}$

> [!Notes]- Mortgage Calculation  
> Initial loan amount: $A$  
> Monthly interest rate: $p$  
> Monthly Payment: $M$  
> Number of months to clear: $n$  
> $f(0) = A$  
> $f(n) = (1 + p)f(n-1) - M$  
> $f(n) = A(1+ p)^n - \frac{M((1+p)^n -1)}{p}$

### Fibonacci Numbers (Second-Order)

$$f_{n} = f_{n-1} + f_{n-2}$$

#### Show whether $n \geq 3, f_{n}> a^{n-2}$, where $a = \frac{1+\sqrt{ 5 }}{2}$

#### Proofing $a_{n} = a \cdot F_{n} + F_{{n-1}}$

### Example: Counting Bit Strings

### Euclid's GCD Algorithm

## Structural Induction

- Balanced Parentheses
- Length

## The Tower of Hanoi
