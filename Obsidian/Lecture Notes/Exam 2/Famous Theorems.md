## Theorem 1: $\sqrt{2}$ is irrational
```ad-example
title: Proof by Contradiction
#### Pf/ Assume $\sqrt{2}$ is rational
Then $\sqrt{2} = \frac{m}{n}, m,n\in\mathbb{Z}, n\neq0$
- Assume $\frac{m}{n}$ is in its simplist form

$\sqrt{2}n = m \implies 2n^2=m^2$
Then we can say that $m^2$ is even $\therefore\ m$ is even.
Then $m=2k,k\in\mathbb{Z}$
$\therefore 2n^2=m^2\to 2n^2 = (2k)^2=4k^2\to n^2 = 2k^2$
Then we can say that $n^2$ is even $\therefore\ n$ is even.
We have a contradiction becuase If both m and n are even, then $\frac{m}{n}$ is not in its simplist form as assumed.
$\square$ Proof by contradiction
```
## Theorem 2: $\forall n\in\mathbb{Z}$ and prime $p$. If $p\mid n$ then $p\nmid (n+1)$
$$
\begin{align} \\
p|n: p\mod n=0 \\
p|(n+1): p\mod n = 1 
\end{align}
$$
## Theorem 3: There are Infinitely Many Primes
```ad-example
title; Proof by Contradiction
This proof is difficult to do without using ocntradiction.
#### Pf/ Assume there are finitely many primes
$A = \set{2,3,5,7,\dots, p}$
Contruct a new integer $N = 2\times3\times5\times\dots\times p + 1,\in\mathbb{Z}$
By $\underline{theorem}$ we learned: $n\ge 2,$ is divisible by a prime.
Let q be a prime such that $q|N$
Because q is prime, $q\in A$, so q is a factor of N.
Therefore we can conclude $q|N-1$ as $N-1=2\times3\times5\times q\times p$
$q|N$ and $q|N-1$ cannot both be true because of theorem 2.
Therefore we can conclude that our assumption is wrong and there are infinitely many primes.
$\square$ Proof by Contradiciton
```
All of the proofs we do are supported by the [[Valid and Invalid Arguments|validity of arguments]]