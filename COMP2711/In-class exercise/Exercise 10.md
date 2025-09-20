## Questions

Two coins are placed in a bag. One of them is a fair coin, while the other is a special coin with tails on both sides. One of the coins is picked from the bag at random and this coin is tossed $2$ times. Let $A_i (i = 1, 2)$ be the event that the coin comes up tail on the i-th toss.

> [!summary] Part A  
> Calculate $P(A_1)$ and $P(A_2)$.

$P(A_1) = P(A_{1} \cap F) + P(A_{1} \cap \bar{F})=\frac{1}{4}+\frac{1}{2} =\frac{3}{4}$

$P(A_2) = P(A_{1})= \frac{3}{4}$

> [!summary] Part B  
> Calculate $P(A_2 | A_{1})$.

$P(A_2 | A_{1})=\frac{P(A_{2} \cap A_{1})}{P(A_{1})}=\frac{3}{4} \times \frac{3}{4} \divsymbol \frac{3}{4}$

> [!summary] Part C  
> Calculate $P(A_2 \cup A_{1})$.

$\frac{3}{4} + \frac{3}{4} - \frac{3}{4} \times \frac{3}{4} = \frac{15}{16}$

> [!summary] Part D  
> Are $A_{1}$ and $A_{2}$ independent? Why?

They are not independent, since $P(A_2) + P(A_{1}) \neq P(A_2 \cup A_{1})$.
