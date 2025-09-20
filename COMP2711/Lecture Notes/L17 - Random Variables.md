V=p(1-p)

## Binomial Distribution

$$
p(x) = {n \choose x} p^x q^{n-x}
$$

$n$: the number of trials (or the number being sampled)  
$x$: the number of successes desired p= probability of getting a success in one trial  
$q=1-p$: the probability of getting a failure in one trial

$$
\sum^n_{{k=0}} {n \choose k} p^k q^{n-k} = (p +q) ^n = 1
$$

### Example

> If a coin is tossed 5 times, using binomial distribution find the probability of  
> **(a) Exactly 2 heads**  
> **(b) At least 4 heads.**

Number of trials = 5

Probability of head: $\frac{1}{2}$  
Probability of tail: $\frac{1}{2}$

For $P(x=2)$, we have ${5 \choose 2} {\left(\frac{1}{2} \right)}^2 \left(\frac{1}{2} \right)^3$

For $P(x\geq 4) = P(x=4) + P(x=5)$, we have ${5 \choose 4} {\left(\frac{1}{2} \right)}^4 \left(\frac{1}{2} \right) + {5 \choose 5} \left(\frac{1}{2} \right)^5$

## Gaussian Distribution

$$
f(x) = \frac{1}{\sqrt{ 2 \sigma^2 \pi }}e^{-\frac{(x - 𝜇)^2}{2 \sigma^2}}
$$

## Infinite Sample Space

> Flip a fair coin until it turns up heads, Let random variable $𝑋 = \text{the number of flips}$.

$$\sum_{x=1}^\infty p(X = x) = 2 + 4 + 8 + \dots = 1$$  
The probability of the event that we get 3 or more flips = $p(X\geq 3) = p(X=3)+p(X=4)+…=\frac{1}{8}+\frac{1}{16}+…=\frac{1}{4}$.

## Geometric Distribution

> Experiment: Flip a fair coin until it turns up heads. Let random variable X = the number of flips.  
> Each coin turns up heads with probability $p$.

#validate

$$
P(X=k) = (1-p)^{k-1}p
$$
$$
P(X \leq x) = 1- (1-p)^x
$$
$$
E(X) = \sum^{\infty}_{k=1} p(1-p)^{k-1} = \frac{1}{p}
$$

### Example

## Expected Value

#cheat-sheet

The expected value (or expectation or mean) of a random variable $X$:

$$
E(X) = \sum_{{x \in S}} p(s)X(s) = \sum_{{x \in X(s)}} p(X=r)r = np
$$

### Examples

> Let $X$ be the number that comes up when a fair dice is rolled. What is the expected value of $X$?

The random variable 𝑋 takes the values $1$, $2$, $3$, $4$, $5$, or $6$. Each has probability $\frac{1}{6}$.

$$
E(X) = \frac{1}{6} 1 + \frac{1}{6} 2 + \frac{1}{6} 3 + \dots + \frac{1}{6} 6 = \frac{7}{2}
$$

## Standard Deviations and Variance

$$
\text{Variance of X}= V(X) = \sum_{s \in S} (X(s) - E(s))^2 p(s) = E((X - E(X))^2)
$$
$$
V(X) = E(X^2) -E(X)^2
$$

## Linearity of Expectations

$$
E(X_{1} + X_{2} + \dots + X_{n}) = E(X_{1}) + E(X_{2}) + \dots + E(X_n)
$$
$$
E(aX + b) = aE(X) + b
$$

### Example: Balls and Bins

> Throw $m$ balls into $n$ bins randomly. How many boxes will be empty in expectation?

### Example: Sorting Insertion

$$
E(X_{i}) = \frac{1}{i} 1 + \frac{1}{i} 2
 + \dots + \frac{1}{i} i$$

$$
\frac{1}{i} (1+ 2+ \dots +i) = \frac{1}{i} \frac{i}{2} (n+1) = \frac{i+1}{2}
$$

$$
\sum^n_{i=2} \frac{i+1}{2} = \frac{n^2 + 3n -4}{2} = \Theta (n^2)
$$

## Big O Notation

Big O, Big Theta, and Big Omega notations are used to estimate the complexity of algorithms.

* Big O provides an upper bound, Big Omega provides a lower bound, and Big Theta provides a tight bound on the growth rate of an algorithm's runtime as the input size increases.
* Logarithmic algorithms are considered very efficient, linear algorithms are good, and exponential algorithms should be avoided.
