https://www.eecs70.org/assets/pdf/notes/n0.pdf
- A set is a well defined collection of objects called elements or members.
	- Objects can be anything, integer, word, cities, and *other sets*
- If two sets are **equal**, they have the same elements
	-  Order and repetition of elements does not matter
- The size of a set is its **cardinality**

###### Subsets / Proper Subsets
- If every element of set A is also in set B, then A is a **subset** of B.
	- Written as A $\subseteq$ B
	- If set A is **strictly** contained in B (A $\subset$ B) then we say that set A is a **proper** subset.
- Example: A = {1, 2, 3} and B = {1, 2, 3, 4, 5}
	- A is both a **subset** and **proper subset** of B
	- B is a **subset** but **not** a **proper subset** of A.
- Empty sets are denoted by {} or $\emptyset$ 
	- Is a **proper subset** of any nonempty set A
	- Is a **subset** of ever set B

###### Intersections and Unions
- The **intersection** of a set A with a set B is written as A $\cap$ B
	- That being the set containing all elements **in both** in A and B
	- Two sets are said to be **disjoint** if A $\cap$ B = 0
- The **union** of a set A and a set B is written as A $\cup$ B
	- That being the set containing all elements **in either** A or B or both
- For example if A is all positive even numbers and B is all positive odd numbers then A $\cap$ B = 0 and A $\cup$ B = $Z^+$

###### Complements
- If A and B are two sets, then the **relative complement** of A in B, or the **set difference** between B and A, written as B - A or, is the set of elements in B, but not in A
	- B - A = {$x \in$ B | x $\notin A$}
	- EXAMPLE: If A = {3, 4, 5} and B = {1, 2, 3}, then B - A = {1, 2}
###### Quantifiers
- $\forall$ "for all" and $\exists$ "exists"
- Example: ($\forall n \in \mathbb{N}$)($n^{2}+n+41$ is prime)
	- This means that for every element "n" in the set of natural numbers $\mathbb{N}$ the output of the function $n^{2}+n+41$ is prime
		- This statement is actually False if you input 41 in n
- Example: ($\exists x \in S$)(P(x)) means "P(x) is true for some x in S"
- S being the *universe*, or the "type of x"
	- N denotes the set of all natural numbers: {0, 1, 2, 3, ...}.
	- Z denotes the set of all integer numbers: {. . . , −2, −1, 0, 1, 2, . . .}.
	- Q denotes the set of all rational numbers: { $\dfrac{a}{b}$ | a, b ∈ Z, b̸ = 0}.
	- R denotes the set of all real numbers.
	- C denotes the set of all complex numbers.
- Quantifiers are not [[commutative]]