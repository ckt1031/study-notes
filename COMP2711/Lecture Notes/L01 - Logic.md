## Propositional Logic

- **Proposition**: a declarative statement either True or False.
- Tautology: a statement which is always True.

### Compound Propositions

- **Negation**: $\neg$, means `NOT`, like **not True** into **False**.
- **Conjunction**: $\land$, means `AND`, `&&` in JavaScript.
- **Disjunction**: $\vee$ means `OR`, ==any value has true value then true, all false then all false==.
- **Exclusive Or**: $\oplus$, ==must be one value be True and one value be False, TT and FF then false, TF and FT be true==.
- **Conditional Statement (Implication)**: $p \rightarrow q$, if p, then q
	- ==If $p$ is false, the $p \rightarrow q$ is always true==.
	- ==If $p$ is true, $q$ should be true in order to make $p \rightarrow q$ be true==.
	- **Example**: $p$: It is raining, $q$: Wet sidewalks.
		- If $p$ is false, it was not raining, sidewalks can be wet or not wet.
		- But if $p$ is true, if sidewalks not wet, then overall is not true
- **Bidirectional Statement**: $p \leftrightarrow q$, $p$ if and only $q$
	- **Example**: $p$: You read the textbook, $q$: You pass the test, in rational, you can only pass the text only if I read the text book. So, it will not be possible for me to fail if I read or pass without reading.
	- In simple: $p \leftrightarrow q$ ==is true either both sides are true or both sides are false==.

## Propositional Equivalences

| Equivalence                                                 | Name                |
| ----------------------------------------------------------- | ------------------- |
| $p \land T \equiv p$ <br>$p \lor F \equiv p$                | Identity laws       |
| $p \lor T \equiv T$ <br>$p \land F \equiv F$                | Domination laws     |
| $p \lor p \equiv p$ <br>$p \land p \equiv p$                | Idempotent laws     |
| $\lnot (\lnot p) \equiv p$                                  | Double negation law |
| $p \lor q \equiv q \lor p$ <br>$p \land q \equiv q \land p$ | Commutative laws    |

| Equivalence                                                                                                          | Name              |
| -------------------------------------------------------------------------------------------------------------------- | ----------------- |
| $(p \lor q) \lor r \equiv p \lor (q \lor r)$ <br>$(p \land q) \land r \equiv p \land (q \land r)$                    | Associative laws  |
| $p \lor (q \land r) \equiv (p \lor q) \land (p \lor r)$ <br>$p \land (q \lor r) \equiv (p \land q) \lor (p \land r)$ | Distributive laws |
| $\lnot(p \land q) \equiv \lnot p \lor \lnot q$ <br>$\lnot(p \lor q) \equiv \lnot p \land \lnot q$                    | De Morgan's laws  |
| $p \lor (p \land q) \equiv p$ <br>$p \land (p \lor q) \equiv p$                                                      | Absorption laws   |
| $p \lor \lnot p \equiv T$ <br>$p \land \lnot p \equiv F$                                                             | Negation laws     |

| Equivalence                                                                                                                                                                                                                                                                                              | Name                               |
| -------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ---------------------------------- |
| $p \to q \equiv \lnot p \lor q$ <br>$p \to q \equiv \lnot q \to \lnot p$ <br>$(p \to q) \land (p \to r) \equiv p \to (q \land r)$ <br>$(p \to q) \lor (p \to r) \equiv p \to (q \lor r)$ <br>$(p \to r) \land (q \to r) \equiv (p \lor q) \to r$ <br>$(p \to r) \lor (q \to r) \equiv (p \land q) \to r$ | Involving conditional statements   |
| $p \leftrightarrow q \equiv (p \to q) \land (q \to p)$ <br>$p \leftrightarrow q \equiv \lnot p \leftrightarrow \lnot q$ <br>$p \leftrightarrow q \equiv (p \land q) \lor (\lnot p \land \lnot q)$                                                                                                        | Involving biconditional statements |
