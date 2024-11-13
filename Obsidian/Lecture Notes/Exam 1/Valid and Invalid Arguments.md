>[!def] Arguments
>Sequence/list of statement forms

## Premises
	For the following examples, statements separated by commas are indicative of multiple statements that make up a given argument
Let ${p\to q,\ q\to r,\ p\therefore r}$
>[!note]
**Note**: If there is a statement that is simply "${p}$", it means that p is true

Premises ${\implies}$ Conclusion of the Argument
>[!def] Validity of an Argument
>An argument is valid if all true premises lead to a true conclusion
#### Valid Arguments
>[!example] Example: Let ${p\to q,\ p \therefore q}$
>
| p | q | ${p \to q}$ | q |
| ---- | ---- | ---- | ---- |
| T | T | T | T |
| T | F | F | F |
| F | T | T | T |
| F | F | T | F |
The first row is a critical law because all premises are true
This example is valid because the critical premesis leads to a true conclusion
#### Invalid Arguments
>[!example] Example: ${r\to (q\land \lnot r),\ q \to (p\lor r) \therefore p \to r}$
>
| p | q | r | ${r\to q\land \lnot r}$ | ${q \to p\lor r }$ | ${p \to r}$ |
| ---- | ---- | ---- | ---- | ---- | ---- |
| T | T | T | T | T | T |
| T | T | F | T | F | F |
| T | F | T | F | T | T |
| T | F | F | T | T | F |
| F | T | T | T | F | T |
| F | T | F | T | F | T |
| F | F | T | T | T | T |
| F | F | F | T | T | T |
This example has critical premesis in the first, fourht, and last two rows becuase all premesis are true.
>This example shows an invalid argument, because not all critical premises lead to a true conclusion

#### Special Cases
>[!summary] Cases
>1. **Generalization:** ${p \therefore p\lor q}$
>2. **Specialization:** ${p\land q \therefore p}$
>3. **Elimination:** ${p\lor q, \lnot p \therefore q}$
>4. **Transitivity:** ${p \to q,\ q\to r \therefore p\to r}$
>5. **Division into Cases:** ${p \lor q \lor w,\ p \to r,\ q \to r,\ w \to r \therefore r}$
>6. **Contradiction Rule:** ${\lnot p \to c \therefore p}$ 
>7. **Modus Pones:** ${p\to q,\ p\therefore q}$
>7b. **Modus Tollens:** ${p \to q,\ \lnot q \therefore \lnot p}$
Rules 7 and 7b are very similar, and aren't really their own rules
## Division into Cases
>[!example] Suppose $x\in\mathbb{Z}$
>- Case 1: X is even
>$x(x+1)$ is even if Case 1.
>- Case 2: X is odd
>Let $x = 2k+1, k\in \mathbb{Z}$
>$x(x+1)$ is even if Case 2.
>	$2(2k+1)(k+1)$ is always even
#### As shown by the example above, the two Cases lead to the same conclusion
	This division of casses is useful for starting large mathematical proofs
# Fallacies
****
>[!def] Converse Error:
$p\to q\not\equiv q\to p$
If Michael breaks the world record, then he will run under 4 minutes.
#### $(a,b)\not=(b,a)$
## The rest of the logical fallacies can be found [[Logic#Important Equivalence Rules|here]].