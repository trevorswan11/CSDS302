## Proof by Contradiction
Want to show a statement s is true...
1. Assume s is false $\therefore\lnot s$ is true
2. Show that $\lnot s$ leads to a contradiction
```ad-def
title: Recall...
$$
\begin{align}
\lnot&s\to c \\
\therefore&\ \ \  s
\end{align}
$$
```
#### Prove that there is no greatest integer
```ad-example
##### Let s = "there is no greatest integer" 
Pf/ Assume s is false
$\lnot s:$ There is a greatest integer N $\checkmark$
Contruct/Create a new integer N' where N' = N + 1 $\in\mathbb{Z}$
But N' > N $\leftarrow$ N is not the greatest as N' = N + 1
$\square$ Proof by Contradiction
```
#### There is no integer that is both even and odd
```ad-example
##### Let s = "There is no integer that is both even and odd"
Pf/ Assume s is false
$\lnot s:$ There is an integer N s.t N is both even and odd
$$
\begin{align}
N =& 2K_1, K_1\in\mathbb{Z} && \text{N is even} \\
N =& 2K_2 + 1, K_2\in\mathbb{Z} && \text{N is odd} \\
2K_1=& 2K_2 +1 && \text{Set N's equal to each other}\\
\therefore K_1 - K_2 =& \frac{1}{2} && \text{Cannot be the case}\\
\end{align}
$$
Therefore, we can conclude that no number can be both even and odd as the difference of any two integers $K_1$ and $K_2$ must also be an integer
```
## Proof by Contrapositive
Want to prove a conditional, it may be easier to prove the contrapositive then the original statement.
1. $p\to q \equiv \lnot q\to\lnot p$
````ad-example
$$
\forall n\in\mathbb{Z}, \text{ If } n^2 \text{ is even, then } n\text{ is even}
$$
Pf/ Determine the contrapositive of the statement
$$
\forall n\in\mathbb{Z}, \text{ If } n \text{ is odd, then } n^2\text{ is odd}
$$
Let $n = 2k+ 1$
$$
\begin{align}
n =& 2k + 1 \\
\therefore n^2 =& 4k^2 + 4k + 1 \\
=& 2(2k^2 + 2k) + 1 \\
\text{Let } c = 2k^2 + 2k, c\in\mathbb{Z} =& 2c+ 1 \\
\end{align}
$$
Pf/ Use Contradidtion
```ad-def
$$
\begin{align}
p\to q\equiv& \lnot p \lor q \\
\lnot(p\to q) \equiv& p\land \lnot q \\
\end{align}
$$
```
$\lnot s: \exists n\in\mathbb{Z}, n^2$ is even and $n$ is odd
Let $n = 2k+1$
$$
\begin{align}
n =& 2k + 1 \\
\therefore n^2 =& 4k^2 + 4k + 1 \\
=& 2(2k^2 + 2k) + 1 \\
\text{Let } c = 2k^2 + 2k, c\in\mathbb{Z} =& 2c+ 1 \\
\end{align}
$$
$2c + 1$ is odd by definition, so $n^2 = 2c+1$, but $n^2$ is even
$\square$ Proved by Contradiction
````
#### $$
\begin{align}
\text{Summary of Proof by Contradiction} \\
\forall x\in D,p\to q\equiv \forall x\in D, \lnot q\to \lnot p
\end{align}
$$
