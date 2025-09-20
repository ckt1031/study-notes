## Combinations

$$
C(n,k) = {n \choose k} = \frac{n!}{k!(n-k)!}
$$

## Combinatorial Proof and Bijection Principle

![](https://www.youtube.com/watch?v=qggFS72uSeo)

![](https://www.youtube.com/watch?v=7mOYew7aJUA)

## Pigeonhole Principle

if $n$ items are put into $m$ containers, with $n > m$, then at least one container must contain more than one item.

![](https://miro.medium.com/v2/resize:fit:676/1*NcXMdHA-6kCSGW7URq07QA.jpeg)

### Proof (By Contradiction)

> A function $f$ from a set with $k + 1$ or more elements to a set with k elements is not one-to-one.

- The challenge is to correctly determine ==what are the objects (pigeons) and the boxes (pigeonholes)==.

#### Examples

Let $a_1, a_2, …, a_{1997}$ represent an arbitrary arrangement of the numbers $1, 2, …, 1997$. Is the product $(𝑎_1 - 1)(𝑎_2 − 2)…(𝑎_{1997} − 1997)$ an odd or even number?

Even numbers times odd numbers is even number, so to get odd numbers, it must be all odd numbers. In each term, Odd - Even numbers must be odd numbers.

$1997/2=998.5$, so we have 998 even numbers (Holes), and 999 odd numbers (Pigeons).

Not enough holes, We will have at least one number with odd - odd = even, so the product must be even.

### Generalised Principle

If $n$ objects are placed into $k$ boxes, then there is at least one box containing at least $\lceil \frac{n}{k} \rceil$ objects.

Minimum number = $(\lceil \frac{n}{k} \rceil -1) \times k +1$

> This is the same as ﬁnding the minimum number $n$ of pigeons such that at least one of the $k$ pigeonholes contain at least $\lceil \frac{n}{k} \rceil$ objects.

#### Proof: Contradiction

#### Examples 1: Cards

How many cards must be selected from a standard deck of $52$ cards to guarantee that at least three cards of the same suit are chosen? How many cards must be selected to guarantee that at least three hearts are selected?

We have 13 cards for each suit, where we have totally 4 suits.

## Combinations

$$
C(n,k) = \frac{n!}{k!(n-k)!}
$$

## Pascal's Identity

$n$ and $k$ be integers, $0 \lt k \lt n$:

$$
{n \choose k} = {n-1 \choose k-1} + {n-1 \choose k}
$$

## Vandermonde's Identity

$$\binom{m + n}{r} = \sum\limits_{k=0}^r \binom{m}{r - k}\binom{n}{k}$$

### Generalized Formula

$$\sum_{k_1+\cdots +k_p = m} {n_1\choose k_1} {n_2\choose k_2} \cdots {n_p\choose k_p} = { n_1+\dots +n_p \choose m }$$
