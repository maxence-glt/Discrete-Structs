
https://www.eecs70.org/assets/pdf/notes/n1.pdf
###### Proposition
- Proposition only T / F
- Common variables are P, Q, R, S...
- Combine propositions
	- *Conjunction* $\land$ ("and") True only when both P and Q are True
	- *Disjunction* $\lor$ ("or") True when at least one of P and Q is True
	- Negation $\neg$ ("not") True when P is false
- The **law of excluded middle** states that for any proposition P either P is true or $\neg$P is False
- Truth tables used for logical equivalence of propositional forms
- DeMorgan's Laws for Negation: distribute and flip
	- $\neg$(P $\land$ Q) $\equiv$ $\neg$P $\lor$ $\neg$Q
	- $\neg$(P $\lor$ Q) $\equiv$ $\neg$P $\land$ $\neg$Q
###### DeMorgan's Laws truth table
	
| P | Q | $\neg$(P $\land$ Q) | $\neg$P $\lor$ $\neg$Q | $\neg$(P $\lor$ Q) | $\neg$P $\land$ $\neg$Q |
| ---- | ---- | ---- | ---- | ---- | ---- |
| T | T | F | F | F | F |
| T | F | T | T | F | F |
| F | T | T | T | F | F |
| F | F | T | T | T | T |
	
###### Implication
- P $\implies$ Q
	- AKA "If P, then Q" or "If P is **True**, Q is **True**"
	- ONLY **False** when P is **True** and Q is **False**
	- P **False** implies nothing
		- P False means Q can be **True** or **False**
	- P can be **True** or **False** when Q is **True**

| P | Q | P $\implies$ Q | $\neg$ P $\lor$ Q |
| ---- | ---- | ---- | ---- |
| T | T | T | T |
| T | F | F | F |
| F | T | T | T |
| F | F | T | T |
$\neg$ P $\lor$ Q    $\equiv$     P$\implies$Q
These are <u>logically equivalent</u>

###### Contrapositive, Converse
https://en.wikipedia.org/wiki/Contraposition
- **Contrapositive** of P $\implies$ Q is $\neg$Q$\implies$$\neg$P
- **Converse** of P $\implies$ Q is  Q $\implies$ P 
- "If the plant pollutes, fish die"
	- If the fish don't die, the plant does not pollute. (**Contrapositive**)
	- If fish die, the plant pollutes. (**Converse**)
- "If you stand in the rain, you get wet"
	- If you did not get wet, you did not stand in the rain. (**Contrapositive**)
	- If you did not stand in the rain, you did not get wet. (**Converse**)
- If P $\implies$ Q and Q $\implies$ P they are **logically equivalent** or P$\iff$Q

| P | Q | $\neg$ P | $\neg$ Q | P$\implies$Q | Q$\implies$P | $\neg$Q$\implies$$\neg$P | P$\iff$Q |
| ---- | ---- | ---- | ---- | ---- | ---- | ---- | ---- |
| T | T | F | F | T | T | T | T |
| T | F | F | T | F | T | F | F |
| F | T | T | F | T | F | T | F |
| F | F | T | T | T | T | T | T |

###### Variables
- These aren't propositions since they have a variable
	- x > 2
	- n is even and the sum of two primes
- Instead we call them *predicates*
