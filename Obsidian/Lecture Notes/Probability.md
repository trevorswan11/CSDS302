## If $m$ pigeons fly into n holes and $m>n$, then at least one hole must contain two or more pigeons.
## Generalized PP (GPP)
$m$ pigeons $\to\ n$ holes and $m>n$, then at least one hole will have at least $k+1$ pigeons.
#### Example
A Bag of markers: 5 red, 8 blue, 10 white, 12 green, 7 yellow (42 total)
Find the minimum number of markers taken from the bag to have at least 5 markers of the same color.
## Expected Value
$$
S=\set{a_1, a_2, a_n}
$$
The expected value is $\mathbb{E}=\sum_\limits{i=1}^na_i\cdot p_i$
## Conditional Probability
S: Sample Space
S': Reduced sample space
$$
Pr(2)=\frac{1}{6}\quad Pr(2)=\frac{1}{3}
$$
- Left expression is in sample space S for all possible die outcomes
- Right expression is for reduced sample space of all even outcomes
#### Notation
$$
Pr(B|A)=\frac{Pr(A\cap B)}{Pr(A)}\quad Pr(B)=\frac{|B|}{|S|}
$$
This means probability of B given A.
****
For finding the chance of rolling two out of even outcomes of die...
$$
Pr(B|A)=\frac{Pr(A\cap B)}{Pr(A)}= \frac{\frac{1}{6}}{\frac{1}{2}}=\frac{1}{3}
$$
Probability of rolling a 2 out of all the possible outcomes is $\frac{1}{6}$ and the probability of rolling an even number is $\frac{1}{2}$ on a 6 sided die.
****
You have a pair of dice of different colors. What is the probability the sum of two numbers is 8, given that both numbers are even.
1. Define a sample Space
$$
S=\set{1\ 1, 1\ 2, 1\ 3, 1\ 4\dots, 6\ 6}
$$
Each position of the sample space has 6 so: $|S|=36$
2. Define possible sums to eight
$$
S'=\set{2\ 6, 4\ 4, 3\ 5}\quad\text{And the other way around!}
$$
Each position here only has 3 choices to sum to 8, so: $\frac{6}{36}=\frac{1}{6}$
$$
Pr(B|A)=\frac{Pr(A\cap B)}{Pr(A)}=\frac{\frac{|A\cap B|}{|S|}}{\frac{|A|}{|S|}}=\frac{\frac{3}{36}}{\frac{9}{36}}=\frac{3}{9}=\frac{1}{3}
$$
## Independent Events
You flip two coins, one coin gets a head and the other is a tail.
- A: first coin is head
- B: second coin is tail
$$
A=\set{HH, HT, TT, TH}
$$
$$
Pr(B|A)=\frac{Pr(A\cap B)}{Pr(A)}=\frac{\frac{|A\cap B|}{|S|}}{\frac{|A|}{|S|}}=\frac{\frac{1}{4}}{\frac{2}{4}}=\frac{1}{2}
$$
Notice that: $Pr(B|A)=\frac{1}{2}$ is the same as $Pr(B)=\frac{1}{2}$
## Bayes Theorem
$$
Pr(A|B)=\frac{Pr(A\cap B)}{Pr(B)}
$$
$$
Pr(B|A)=\frac{Pr(A\cap B)}{Pr(A)}
$$
We can do some basic algebraic manipulations on the two equations above. The theorem says:
$$
\begin{align} \\
Pr(A|B)\cdot Pr(B)=Pr(B|A)\cdot Pr(A) \\ \\ \\
Pr(A|B)=\frac{Pr(B|A)\cdot Pr(A)}{Pr(B)}
\end{align}
$$
#### Example: Cats
There is a test for allergy to cats, test accuracy is 80% (means that for people that really have allergy, 80% of the time "yes", for people without allergy, 20% also say "yes" *false pos*)
$$
Pr(Allergy|\text{Yes})=\frac{Pr(\text{Yes}|Allergy)\cdot Pr(Allergy)}{Pr(\text{Yes})}
$$
Suppose that only 1% of the population has a cat allergy, then:
- Case 1: $1\%\times80\%$
- Case 2: $99\%\times20\%$
Adding these two together yields a success rate of $20.6\%$.
Improving the product greatly will increase the percentage reduced false positives
## Permutation
Order is important here!
$$
P(n,r)=\frac{n!}{(n-r)!}
$$
#### Permutations with Sets of Indistinguishable Objects
Where there are $n$ total objects and $n_k$ indistinguishable objects of type $k$:
$$
\frac{n!}{n_1!n_2!n_3!\dots n_k!}
$$
## Combinations
#### r-Combination
A set of n elements is a subset that contains r of the n elements
****
Order is not important here!
$$
C(n,r)= {n\choose r}=\frac{n!}{r!(n-r)!}
$$

