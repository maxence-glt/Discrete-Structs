https://www.eecs70.org/assets/pdf/dis00a.pdf

1. **Propositional Practice** - Convert the following English sentences into propositional logic and the following propositions into English. State whether or not each statement is true with brief justification
	- There is a real number which is not rational.
		- ($\exists x \in R$)($x \notin Q$)
		- True because pi
	- All integers are natural numbers or are negative, but not both
		- ($\forall x \in Z$)((($x \in N$) $\lor$ ($x < 0$)) $\land$ $\neg$(($x \in N$) $\land$ ($x < 0$)))
		- True
	- If a natural number is divisible by 6, it is divisible by 2, or it is divisible by 3
		- ($\forall x \in Z$)((6 | x) $\implies$ ((2 | x) $\lor$ (3 | x)))
		- True
	- ($\forall x \in Z$)($x \in Q$)
		- Every integer x is a rational number
		- True
	- ($\forall x \in Z$)((($2 | x$) $\lor$ ($3 | x$)) $\implies$ ($6 | x$))
		- Every integer x that is divisible by 2 or 3 is divisible by 6
		- False
	- ($\forall x \in N$)((x > 7) $\implies$ (($\exists a, b \in N$)(a + b = x)))
		- Every natural number x that is greater than 7 is such that there exists natural numbers a and b that sum to equal x
2. **Truth Tables** - Determine whether the following equivalences hold, by writing out truth tables. Clearly state whether or not each pair is equivalent.
	 - $P \land (Q \lor P) \equiv P \land Q$ is **not equivalent**
	 - $(P \lor Q) \land R \equiv (P \land R) \lor (Q \land R)$ is **equivalent**
	 - $(P \land Q)\lor R \equiv (P \lor R) \land (Q \lor R)$ is **equivalent**
	
| P | Q | $P \land (Q \lor P)$ | $P \land Q$ |
| ---- | ---- | ---- | ---- |
| T | T | T | T |
| T | F | T | F |
| F | T | F | F |
| F | F | F | F |

| P | Q | R | $(P \lor Q) \land R)$ | $P \land R$ | $Q \land R$ | $(P \land R) \lor (Q \land R)$ |
| ---- | ---- | ---- | ---- | ---- | ---- | ---- |
| T | T | T | T | T | T | T |
| T | F | T | T | F | F | T |
| T | T | F | F | F | F | F |
| T | F | F | F | F | F | F |
| F | T | T | T | F | T | T |
| F | F | T | F | F | F | F |
| F | T | F | F | F | F | F |
| F | F | F | F | F | F | F |

| P | Q | R | $(P \land Q)\lor R$ | $(P \lor R)$ | $(Q \lor R)$ | $(P \lor R) \land (Q \lor R)$ |
| ---- | ---- | ---- | ---- | ---- | ---- | ---- |
| T | T | T | T | T | T | T |
| T | F | T | T | T | T | T |
| T | T | F | T | T | T | T |
| T | F | F | F | T | F | F |
| F | T | T | T | T | T | T |
| F | F | T | T | T | T | T |
| F | T | F | F | F | T | F |
| F | F | F | F | F | F | F |

3. **Implication** - Which of the following implications are always true, regardless of P? Give a counterexample for each false assertion (i.e. come up with a statement P(x, y) that would make the implication false).
	- $\forall x \forall y P(x, y) \implies \forall y \forall xP(x, y)$
		- This is **always true**, doesn't matter the order of the foralls
	- $\forall x \exists y P(x, y) \implies \exists y \forall xP(x, y)$
		- This is **not always true**, since it states that for all x there exists y such that P(x, y), which is different from there exists y such that for all x there is P(x, y)
	- $\exists x \forall y P(x, y) \implies \forall y \exists xP(x, y)$
		- This is **always true**, "there exists x where all y..." == "for all y there exists x..."