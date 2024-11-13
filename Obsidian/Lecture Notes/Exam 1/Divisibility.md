```ad-def
n is divisible by d if $n=k\cdot d, k\in \mathbb{Z},$ d|n
```
## Proof
```ad-theory
$$
\begin{align}
m=&k\cdot p_1,p_1\in\mathbb{Z} \\
n=&m\cdot p_2, p_2\in\mathbb{Z} \\
n=&m\cdot p_2=k\cdot p_1\cdot p_2 \to k|n \\
\end{align}
$$
```

#### Example
$$
\begin{align}
\forall m,n\in\mathbb{Z}, \text{ if } n|m, m|n \\
\text{m=n} && \text{false} \\
\end{align}
$$
# Most Important Theorem in this class
```ad-theory
title: Theorem: Divisibility of Prime
Any integer greater than 1 is divisible by a prime
```

## Euclid's Theorem
```ad-theory
$$
\begin{align}
\forall a,b\mathbb{Z},&& &\text{and a prime p} \\
\text{If } p|ab,&& &\text{then } p|a \text{ or } p|b
\end{align}
$$
The converse of this is also true.
```
```ad-example
Let $a,b\in\mathbb{Z}$ and p is prime and p|ab.
Show that p|a$\lnot$p|b
#### Case 1: p|a
Done!
#### Case 2 p$\nmid$a $\leftarrow$ p does not divide a 
$a=p \cdot k + s \qquad \text{ A remainder s}$ where $\ge s<p$
##### Proof for Case 2
$$
\begin{align}
\text{Multiply Both sides by b}& && a\cdot b = (p\cdot k + s)\cdot b \\
\text{Simplify}& && pkb + sb = pm, m\in\mathbb{Z} \\
\text{Solve for m}& && pks + sb = pm \implies m = kb + \frac{sb}{p}, \frac{sb}{p}\in\mathbb{Z} \\
\text{Conclusion}& &&\therefore p|b
\end{align}
$$
If p does not divide a, then p must divide b
```
# Prime Numbers
$$
\begin{align}
&\forall n\in\mathbb{Z}^+, n\ge 2 \\
&n = P_1\ P_2\dots P_k \\
&\text{Where }P_i\text{ is prime.} \\
&\text{This factorization is }\boxed{\text{Unique}}
\end{align}
$$
#### The fundamental theorem of arithmetic and the unique factorization theorem
although we might look at $999\to 1000$ as being very close to each other, prime factorization reveals $999\to1107$ is a better relationship
$$
\begin{align} \\
999=&\ 3\times3\times3\times37 \\
1107=&\ 3\times3\times3\times41\\
\end{align}
$$
```ad-theory
title: Proof of Uniqueness
Assume that there exists an n, $n=P_1,P_2\dots P_k = q_1,q_2\dots q_l$
#### Case 1, By Euclids:
$$
\begin{align}
P_1|&a \\
\text{or }P_1|&q_1 \\
P_1 =& q_1 \\
\end{align}
$$
#### Case 2, By Euclids:
$$
\begin{align}
P_1|&b \\
\text{or }P_1|&q_2,q_3\dots q_l \\
\dots
\end{align}
$$
#### Case 2.1
$$
P_1|q_2 \to P_1=q_2
$$
#### Case 2.2
$$
P_1|q_3,q_3\dots q_l
$$
$$
\text{Eventually, we can conclude that $P_1 = q_l$}
$$
```

```ad-def
title: Proving Uniqueness again
$\forall n \ge 2$
$n = p_1 p_2\dots p_k\leftarrow$ Unique
### Proof: 
Let $n\in\mathbb{Z}, n\ge 2$
#### Case 1: n is prime
$\square$

#### Case 2: n is not prime
$$
\begin{align}
p_1|&n && p_1\text{ is prime} \\
\end{align}
$$
#### Case 2.1 $\frac{n}{p_1}$ is prime
$$
\begin{align}
n = p_1& && \frac{n}{p_1}
\end{align}
$$
$$\dots$$
```
