>[!def] Statements
>A statement is a structure that is either true or false, but not both.
>- Statements are represented by "p" or "q"
>- ${p\land q}$ means p *and* q
>- ${p \lor q}$ means p *or* q
>- ${\lnot p}$ or ${\sim p}$ means *not* p
>	- I will be *exclusively* using ${\lnot}$
**Example:** ${x+3>5}$ for ${x\in \mathbb{Z}}$ if ${}x\ge 10$, true
#### Truth Tables can be used to describe the relationship between statements
>[!def] Important Terminology
**Tautology:** A tautology "$t$" is a statement form that is *always* true.
>
>
| p | ${\lnot p}$ | ${p\land \lnot p}$ |
| ---- | ---- | ---- |
| T | F | T |
| F | T | T |
**Contradiction:** A contradiction "$c$" is a statement form that is *always* false.
>
| p | ${\lnot p}$ | ${p\land \lnot p}$ |
| ---- | ---- | ---- |
| T | F | F |
| F | T | F |
## **Important:**${\lnot (p\land q) \equiv \lnot p \lor \lnot q}$
	This is also known as De Morgan's Law, as shown in the Equivalence Laws
	
| p | q | ${p\land q}$ | ${\lnot(p\land q)}$ | ${\lnot p \lor \lnot q}$ |
| ---- | ---- | ---- | ---- | ---- |
| T | T | T | F | F |
| T | F | F | T | T |
| F | T | F | T | T |
| F | F | F | T | T |
# Equivalence and Laws
****
>[!note] Equivalence
>Two statement forms "${\equiv}$" are logically equivalent if they have identical truth values
	
Normal Computers can do ${2^4}$ operations while Quantum computing is *not* limited
>[!theory] Theorem 2.1: Equivalence Laws
>1. **Commutative Law:** ${p\land q\equiv q\land p}$
>	This works with ${\lor}$ as well
>2. **Associative Law:** ${(p\land q)\land r\equiv p\land(q\land r)}$
>3. **Distributive Law:** ${p\land(q\lor r)\equiv(p\land q)\lor (p\land r)}$
>4. **Identity Law:** ${p\land t \equiv p,\ p\lor c \equiv p}$
>5. **Negation Law:** ${p\lor \lnot p \equiv t,\ p\land c \equiv p}$
>6. **Double Negation Law:** ${\lnot(\lnot p)\equiv p}$
>7. **Idempotent Law:** ${p\land p\equiv p,\ p\lor p \equiv p}$
>8. **Universal Bound Law:** ${p\lor t \equiv t,\ p\land c\equiv  c}$
>9. **De Morgan's Law:** ${\lnot(p\lor q)\equiv \lnot p\land \lnot q,\ \lnot(p\land q)\equiv \lnot p\lor \lnot q}$
>10. **Absorption Law:** ${p \lor(p\lor q)\equiv p,\ p\land(p\lor q)\equiv p}$
>11. **Negations of $t$ and $c$:** ${\lnot t \equiv c,\ \lnot c \equiv t}$
>*Note: These are given on exams, you just need to know how to apply them*
## Prove: ${\lnot(\lnot p\land q)\land(p\lor q)\equiv p}$
*Note: LHS means Left Hand Side in Proofs*
$$
\begin{align}
LHS & \equiv (\lnot(\lnot p)\lor \lnot q)\land (p\lor q) && (by\ 9)\\
& \equiv (p\lor \lnot q)\land(p \lor q) && (by\ 6) \\
& \equiv p\lor(\lnot q \lor q) && (by\ 3) \\
& \equiv p\lor c \\
& \equiv p \\
& \square
\end{align}
$$
>[!example] Example: Equivalence
>"If it rains tomorrow, then the school is canceled"${\equiv}$"If the school doe not cancel, then it does not rain tomorrow"

# Important Equivalence Rules
>[!def] Suppose ${p\rightarrow q}$
>1. **Converse:** ${q\rightarrow p \not\equiv p\rightarrow q}$
>2. **Inverse:**  ${\lnot p \rightarrow \lnot q \not\equiv p\rightarrow q}$
>3. **Contrapositive:** ${p\to q\equiv \lnot q \to \lnot p}$
>4. **Negation:** $\lnot(p\to q)\equiv p\land \lnot q$

#### The Converse reverses p and q: $p\to q$ becomes $q\to p$.
#### The inverse negates both sides: $p\to q$ becomes $\lnot p \to \lnot q$

>[!example] Example: False Equivalence
>"If Michael breaks the world record, then he will run under 4 minutes" ${\not\equiv}$ "If under 4' then breaks WR"
## Hypotheses and Conclusions 
>[!def] 
>If ${p,\ q\lor p \implies q,\ p\to q}$
>- p is sufficient condition of q
>- q is necessary condition of p
>p: hypothesis
>q: conclusion
#### Contrapositive Form: ${\lnot q \to \lnot p \equiv p\to q}$
>[!tldr] Trick
>The statement for $p\to q$ is only false when p is true and q is false. It is true in *all* other situations.