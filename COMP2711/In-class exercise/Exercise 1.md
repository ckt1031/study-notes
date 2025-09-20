> [!summary] Question 1  
> Construct a truth table for the statement $\neg((p \lor q) \land \neg p) \land \neg p$

| $p$ | $q$ | $p \lor q$ | $\neg p$ | $(p \lor q) \land \neg p$ | $\neg((p \lor q) \land \neg p)$ | $\neg((p \lor q) \land \neg p) \land \neg p$ |
|---|---|---|---|---|---|---|
| T | T | T | F | F | T | F |
| T | F | T | F | F | T | F |
| F | T | T | T | T | F | F |
| F | F | F | T | F | T | T |

> [!summary] Question 2  
> Are the following statements logically equivalent:  
> $(\neg p \land (\neg p \land q)) \lor (p \land (p \land \neg q))$  
> $(\neg p\land q)\lor(p \land\neg q)$

$((\neg p \land (\neg p \land q)) \lor (p \land (p \land \neg q))$  
$\equiv ((q \land \neg p) \land q) \lor ((\neg q \land  p) \land \neg q))  -  \text{Associative laws}$  
$\equiv (\neg p \land q) \lor (p \land \neg q) - \text{Idempotent laws}$
