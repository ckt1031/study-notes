## Reminder

- **Poker:** Know definitions and be able to *derive* the probabilities for various hands.
- **Probability Distributions:** Understand what makes a distribution valid.
- **Independence:** Be able to identify independent events using the mathematical definition and the logic that one event does not affect the others' probabilities
- **Conditional Probability:** Master the formula and understand how it modifies the sample space. Know when to use the law of total probability or its corollaries

## Introduction to Poker

> Ref: https://en.wikipedia.org/wiki/List_of_poker_hands

- **Royal flush**: J, K, Q, 10, A

![image](https://obsidian-img-studies.tsun1031.xyz/2024/10/07/135367bc02b52076afbc6a813c592faf30fbda1124395afbb69dd2d87a5950e5.png)

![image](https://obsidian-img-studies.tsun1031.xyz/2024/10/07/deb55bf8e212db270dfd7d762e969de7300e6941fe99ce9d75b3b513dd2c6ade.png)

![image](https://obsidian-img-studies.tsun1031.xyz/2024/10/07/796b8a2cb1741448b9707aa9b2f5fff419485d950c25f1504d8a03cf6b32bd60.png)

![image](https://obsidian-img-studies.tsun1031.xyz/2024/10/07/914087bc890984b2135c78d67dfdf65c0887392b0c5eae7aee196fc9275a5e19.png)

## Probability Basics

**Definition of Probability:** The probability of an event E is defined as the number of favorable outcomes divided by the total number of possible outcomes in the sample space S.

$$P(E) = \frac{|E|}{|S|}$$

- Where $|E|$ is the number of outcomes in event $E$ and $|S|$ is the size of the sample space.

## Poker Hand Probabilities

### Basic Deck Info

- 52 cards in a deck; 4 suits (diamonds, hearts, spades, clubs); 13 ranks (Ace, 2-10, Jack, Queen, King).

### Example Calculations

- **Hand with Ace of Spades and King of Spades:**
	- The remaining 3 cards can be any of the remaining 50 cards
	- Number of ways: $\binom{50}{3}$
	- Probability: $\frac{\binom{50}{3}}{\binom{52}{5}}$
- **Hand with Exactly One Ace:**
	- Choose 1 of 4 Aces: $\binom{4}{1}$
	- Choose 4 of the 48 non-Ace cards: $\binom{48}{4}$
	- Probability: $\frac{\binom{4}{1} \cdot \binom{48}{4}}{\binom{52}{5}}$
- **Hand with Five Different Kinds (Numbers):**
	- Choose 5 different ranks from 13: $\binom{13}{5}$
	- For each chosen rank, choose one of the four suits: $4^5$
	- Probability: $\frac{\binom{13}{5} \cdot 4^5}{\binom{52}{5}}$
- **Royal Flush:**
	- 10, Jack, Queen, King, Ace of the same suit.
	- 4 possible royal flushes (one per suit).
	- Probability: $\frac{4}{\binom{52}{5}}$
- **Straight Flush:**
	- 5 consecutive cards of the same suit, *excluding* royal flush.
	- 9 possible starting ranks (Ace through 9).
	- For each of the 9 starting ranks, there are four suits possible.
	- Number of combinations: $9 * 4$
	 - Probability: $\frac{9 \cdot 4}{\binom{52}{5}}$
- **Straight:**
	- 5 consecutive cards of any suit, excluding straight and royal flush.
	- 10 possible starting ranks (Ace through 10).
	- Each card can have 4 possible suits.
	- Total is $10 \cdot 4^5$
	- Need to exclude the number of royal flush and strict flush.
	- Probability: $\frac{10 \cdot 4^5 - 4 - 36}{\binom{52}{5}}$
- **Flush:**
	- 5 cards of the same suit, excluding royal/straight flush.
	- Choose 5 cards of any kind of the 13 different ranks: $\binom{13}{5}$
	- Choose 1 of 4 suits.
	- Need to exclude the number of royal flush and strict flush.
	- Probability: $\frac{\binom{13}{5} \cdot 4 - 4 - 36}{\binom{52}{5}}$
- **Three of a Kind:**
	- Choose a rank (1 of 13): $\binom{13}{1}$
	- Choose 3 suits for that rank: $\binom{4}{3}$
	- Choose 2 different remaining ranks: $\binom{12}{2}$
	- Choose 1 suit for each of the 2 remaining ranks: $4^2$
	- Probability: $\frac{\binom{13}{1} \binom{4}{3} \binom{12}{2} \cdot 4^2}{\binom{52}{5}}$
- **Two Pairs:**
	- Choose 2 ranks for the pairs: $\binom{13}{2}$
	- Choose 2 suits for each rank: $\binom{4}{2}^2$
	- Choose 1 of remaining card: $44$
	- Probability: $\frac{\binom{13}{2} \binom{4}{2}^2 \cdot 44}{\binom{52}{5}}$

## Probability Distributions

A probability distribution assigns a probability to each possible outcome in the sample space.

### Requirements for a Valid Probability Distribution

- $0 \leq P(x) \leq 1$ for all outcomes x in the sample space.
- $\sum_{x \in S} P(x) = 1$, i.e., the sum of all probabilities over the sample space equals one.

### Uniform Distribution

All outcomes have equal probability (e.g., fair die).

### Non-Uniform Distribution

Outcomes have different probabilities (e.g., loaded die).

## Independence of Events

Two events E and F are independent if the occurrence of one does not affect the probability of the other.

### Mathematical Condition

$$P(E \cap F) = P(E) \cdot P(F)$$

### Pairwise Independence

Each pair of events is independent

### Mutual Independence

All combinations of events are independent. Mutually independent is stronger than pairwise.

For example, $P(E_1 \cap E_2 \cap E_3) = P(E_1)P(E_2)P(E_3)$.

### Example

The coin flip example demonstrates a scenario where events are pairwise independent but *not* mutually independent.

## Conditional Probability

The probability of an event E given that event F has occurred.

$$P(E|F) = \frac{P(E \cap F)}{P(F)}$$

- Where $P(E|F)$ is probability of E given F

### Corollary 1 (Intersection)

$$P(E \cap F) = P(F) \cdot P(E|F)$$

### Corollary 2 (Chain Rule)

$$P(E_1 \cap E_2 \cap \dots \cap E_n) = P(E_1)P(E_2 | E_1) P(E_3 | E_1 \cap E_2) … P(E_n | E_1 \cap … \cap E_{n-1})$$

### Example 1: Bits

- Probability of having two consecutive zeros given that the first bit is zero.
- Solved both using logic and the conditional probability formula, yielding the same result: 5/8.

### Example 2: True/False Exam

Probability of answering correctly given an 80% knowledge of the material and guessing otherwise,

Calculated using the law of total probability and conditional probabilities.

$$\begin{align}
P(\text{Correct})  & = P(\text{Correct}|\text{Know})P(\text{Know}) + P(\text{Correct}|\text{Not Know})P(\text{Not Know})  \\
 & = (1)(0.8) + (0.5)(0.2) = 0.9
\end{align}$$


## Birthday Paradox

**Question**: What is the minimum number of people needed to guarantee that two of them will share the same birthday and the maximum number of people to make sure the probability at least two people has same birthday is greater than 1/2

For the guaranteed scenario, the number is 367 according to pigeonhole principles

The complement: No two people has the same birthday

### Probability Calculation

- $P(\text{No Same Birthday}) = \frac{366}{366} \cdot \frac{365}{366} \cdot \frac{364}{366} \cdot \dots \cdot \frac{366-n+1}{366}$
- $P(\text{At Least One Same Birthday}) = 1 - P(\text{No Same Birthday})$

### Minimum Number

- The minimum number to satisfy the condition is 23 people

## Independence Revisit

- If E and F are independent then $P(E|F) = P(E)$
- Independent means one event doesn't affect other event's probability.
