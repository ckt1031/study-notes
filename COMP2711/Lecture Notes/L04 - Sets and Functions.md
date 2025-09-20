- A set is an unordered collection of objects
- Null or empty set: $\emptyset$ or $\{\}$
- Subset of: ⊆

## Cardinality of Finite Sets

Denoted by $| S |$, means the number of elements in $S$.

## Power Set

$$
S = \{1,2,3\}
$$

$$
P(S) = \{\{\}, \{1\}\, \{2\}, \{3\}, \{1, 2\}, \{2, 3\}, \{1, 3\}, \{1, 2, 3\} \}
$$

$$
|P(S)| = 2^{|s|}
$$

### Tuple

$$
(a_{1}, a_{2}, \dots, a_{n})
$$

## Cartesian Product

$$
A × B = \{ (a,b ) | a \in A \text{ and } b \in B \}
$$

Kind of matching, get all possibilities.

The tuple inside is in order, $(1, 2)$ and $(2, 1)$

$$
A = \{\text{James}, \text{Peter}\}, B = \{A, B, C\}
$$

$$
𝐴 × 𝐵 = \{ (\text{James}, A), (\text{James}, B), (\text{James}, C), (\text{Peter}, A), (\text{Peter}, B), (\text{Peter}, C)
\}
$$

## Union, Intersection, and Cardinality

$|A \cup B| = |A| + |B| - |A \cap B|$

## Differences

> set containing those elements that are in 𝐴 but not in 𝐵

The **complement** of a Set $A$, denoted by $\overline{A}$, or just $U - A$

$$
\{1 , 3 , 5\} − \{1 , 2 , 3 \} = \{5\}
$$

## Set Identities and Laws

| Identity                                                                                                         | Name              |
| ---------------------------------------------------------------------------------------------------------------- | ----------------- |
| $A \cup (B \cup C) = (A \cup B) \cup C$<br>$A \cap (B \cap C) = (A\cap B) \cap C$                                | Associative laws  |
| $A \cap (B \cup C) = (A \cap B) \cup (A \cap C)$<br>$A \cup (B \cap C) = (A \cup B) \cap (A \cup C)$             | Distributive laws |
| $\overline{A \cup B} = \overline{A} \cap \overline{B}$<br>$\overline{A \cap B} = \overline{A} \cup \overline{B}$ | De Morgan's laws  |
| $A \cup (A \cap B) = A$<br>$A \cap (A \cup B) = A$                                                               | Absorption laws   |
| $A \cup \overline{A} = U$<br>$A \cap \overline{A} = \emptyset$                                                   | Complement laws   |

## Functions

onto, correspond

![image](https://obsidian-img-studies.tsun1031.xyz/2024/10/16/5bee9b85b584e31c03e1187151bc100ebf0e3dce6baf0205c415d4379cd11679.png)

- Injective Function: one-to-one (Unique)
- Surjective Function: onto (Every B must have some A)
- Bijective: onto and one-to-one
- Inverse Function: one-to-one correspondence

## Infinity Sets

$$|N| = ℵ_{0}$$
- $N \ (\text{Natural Number})$ is countable.  
- To know if the set is countable, $|S| =n, n \in N$ or $|S| = |N|$, otherwise it is uncountable.
- Proof/explain why, by telling is it one-to-one and onto

### Examples

1. is $Z^+$ countable?, $f: N \to Z^+$, one-to-one: $f(x) = x+1$

### Real Numbers

> $R^+$ is uncountable

no on to = strictly bigger

## Schröder-Bernstein Theorem

$|S| < |P(S)|$

## Cantor's Diagonalisation

> A technique that shows that the integers and reals cannot be put into a one-to-one correspondence (i.e., the uncountably infinite set of real numbers is "larger" than the countably infinite set of integers). Cantor's diagonal argument applies to any set S, finite or infinite.
