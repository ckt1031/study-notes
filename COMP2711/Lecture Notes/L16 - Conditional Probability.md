## Reminder

* Bayes' Theorem is essential for "swapping" conditional probabilities and calculating posterior probabilities.
* Posterior probability is often more meaningful in real-world applications.
* Be careful when applying Bayes' Theorem, especially in complex scenarios like the Monty Hall problem.
* Understanding the problem setup and deriving the probabilities is crucial.
* ==Remember to include Bayes' Theorem and the conditional probability formula on your cheat sheet!==

## Conditional Probability

$$P(A \mid B) = \frac{P(A \cap B)}{P(B)}$$  
* $P(E|F)$ is the probability of event E given event F.
* $P(E \cap F)$ is the probability of both E and F occurring.
* $P(F)$ is the probability of event F occurring.

### Example: Rolling Dice

* Probability of getting a 2: 1/6  
* Probability of getting a 2 given the result is even: 1/3

### Other Examples

* $P(\text{A+} | \text{score} > 80)$: Probability of getting A+ given a score > 80.  
* $P(\text{score} > 80 | \text{A+})$: Probability of score > 80 given an A+.
* $P(\text{Test Positive} | \text{Disease})$: Probability of testing positive given you have the disease (Easier to obtain).
* $P(\text{Disease} | \text{Test Positive})$: Probability of having the disease given you tested positive (More difficult to obtain).

---

$$p(E \cap F) = p(F)p(E|F)$$

## Bayes' Theorem

Suppose E and F are events from space S, such that $p(E) > 0$ and $p(F) <0$, then:

$$
p(F|E) = \frac{p(E|F)p(F)}{p(E|F)p(F) + p(E|\bar{F})p(\bar{F})}
$$

> [!note] proof  
> $$p(E \cap F) + p(E \cap \bar{F}) = p(E)$$

### Generalized Theorem

Suppose that $E$ is an event from a sample space $S$ and that $F_{1}, F_{2}, \dots,F_{n}$ are mutually exclusive events such that $\bigcup_{i=1}^{n} F_i = S$. Assume that $p(E) \neq 0$ and $p(F_{i}) \neq 0$ for $i = 1,2,\dots,n$.

$$p(F_j|E) = \frac{p(E|F_j)p(F_j)}{\sum_{i=1}^n p(E|F_i)p(F_i)}.$$

### Applications

* **Medical Testing:** Determining the probability of actually having a disease given a positive test result.
* **Spam Filtering:** Classifying emails as spam or not spam based on the presence of certain words.
* **General Classification Problems:** Using AI to classify data into different categories.
* **Monty Hall Problem:** Determining the optimal strategy in the Monty Hall game.

## More Examples

### Breathalyzer Example

* Error rate of 5% (5% chance of detecting a sober driver as drunk, 5% chance of not detecting a drunk driver).
* 1 in 1000 drivers are drunk.
* We want to find $P(\text{Drunk} | \text{Test Positive})$, which is different from $P(\text{Test Positive} | \text{Drunk})$.
* Bayes' Theorem helps us swap them.
* Result: If you test positive, there's only a 2% chance you're actually drunk, highlighting the importance of posterior probability.

### Box and Ball Example

* Two boxes, each with different numbers of red and other balls.
* We want to find $P(\text{Box 1} | \text{Red Ball})$.
* Bayes' Theorem helps us swap from $P(\text{Red Ball} | \text{Box 1})$.

### COVID Testing Example

* False negative rate: 1%
* False positive rate: 0.5%
* 1 in 100,000 people have the disease.
* We want to find $P(\text{COVID} | \text{Test Positive})$ and $P(\text{COVID} | \text{Test Negative})$.
* Result: If you test positive, the chance of having COVID is low, but if you test negative, the chance of having COVID is very low.

### Spam Filtering Example

* Classifying emails as "bad" or "good" based on keywords (e.g., "Rolex").
* We want to find $P(\text{Bad Message} | \text{Keyword "Rolex"})$
* Bayes' Theorem helps us swap from $P(\text{Keyword "Rolex"} | \text{Bad Message})$.
* Result: High probability of a bad message when the word "Rolex" is present.

### DVD Player Example (Multiple Companies)

* Three companies (A, B, C) producing DVD players with different defect rates.
* We want to find $P(\text{Company A} | \text{Defect})$.
* Uses the generalized Bayes' Theorem.

### Monty Hall Problem

* Three doors, one with a prize.
* You pick a door, the host opens a door without the prize.
* Should you switch?
* Bayes' theorem is used to calculate the probability of winning if you stick with your original choice vs. switching.
* **Original Setup:** Switching increases your chance of winning to 2/3.
* **Variant Setup:** The probability of the prize being behind each door is not uniform.
* **Optimal Strategy:** The optimal strategy depends on the probabilities of the prize being behind each door and which door the host opens.
* **Cheat Sheet Reminder:** *Pay close attention to the Monty Hall problem, as it's often on exams!*
