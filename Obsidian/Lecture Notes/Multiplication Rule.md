## Possibility tree
#### Definition/Sketch
![[Possibility Tree|700]]
#### Probability of an Event E
$$
P_r(E)=\frac{|E|}{|S|}
$$
where S is the *sample space* $e.g \set{AA,BB,ABB,\dots,ABABA}$ for above example
#### Revisit Example:
What is the probability that A and B played 5 games?
$$
P_r(E)=\frac{\text{Nodes with 5 games}}{\text{Number of Games Total}}=\frac{4}{10}=40\%\leftarrow\text{unbiased data}
$$
## Monte Carlo Simulations
![[Monte Carlo Example|500]]
Because the dots are placed randomly, you can observe that there about 75 dots inside the shape out of the total 100 placed on the group as a whole. This allows us to estimate the area of the arbitrary shape to be:
$$
A\approx25\times\frac{75}{100}
$$
This expression is just a percentage of the total area of the square to derive the area of the inner shape.
## Multiplication Rule
If there is a sequence of $k$ positions to be filled.

| **Position** | **Number of ways to fill** |
| ------------ | -------------------------- |
| 1            | $n_1$                      |
| 2            | $n_1$                      |
| $\vdots$     | $\vdots$                   |
| $k$          | $n_k$                      |
The Multiplication rule says that the total number of wats to fill all $k$ positions is:
$$
n_1\times n_2\times\dots\times n_k=\prod_\limits{i=1}^k n_i
$$
#### Example: 4-digit pin
![[Mult Rule with pin]]
$10^4$ possible 4-digit combinations here.
## Permutation
A permutation of a set of elements is an $\underline{\underline{\text{ordering}}}$ if the elements.
$$
\text{Given a set: }A=\set{a,b,c}
$$
![[abc permutation|500]]
#### Theorem
If the number of elements in a, $|A|=n$, the number of permutations $p(n)$ of A is $n!$.
#### Definition: r-permutations
If $|A|=n$, for $r\le n$
r-permutation $p(n,r)$ is an ordering of r elements of n elements.
#### Theorem: r-permutations
$$
n\cdot(n-1)\dots(n-r+1)=\frac{n!}{(n-r)!}
$$
## Addition Rules
#### Theorem 9.3.1: Addition Rule
If $\set{A_1,A_2,A_3\dots A_k}$ is a partition of $A$. Then:
$$
|A|=\sum_\limits{i=1}^k |A_i|
$$
#### Example:
How many possible passwords consisting of up to 3 alphabets?
Three Cases:
1. Length 1
2. Length 2
3. Length 3
Let $A_1, A_2, \text{ and }A_3$ be 3 partitions of $A$ which correspond to the three cases respectively.
$$
\therefore |A|=|A_1|+|A_2|+|A_3|=26+26^2+26^3
$$