1. even, $n\in \mathbb{Z}, n=2k, k\in\mathbb{Z}$
2. odd, $n = 2k+1$, where $k\in\mathbb{Z}$
3. prime
	n is prime if 1 and n are the only factors of n
4. n is composite is it is not prime
	$n = k\cdot S$ where $k,S\in\mathbb{Z},1<k<n, and\ 1<s<n$
5. $x\in\mathbb{Q}\text{ if } x=\frac{m}{n}$ where $m,n\in\mathbb{Z}, n\not=0$
6. $x\not\in \mathbb{Q}$
## Showing $\forall x\in D, p(x)$, the Universal Statement, is true
1. **Brute force Method**
2. **Generating from generic portable**
3. **Mathematical Induction**
#### Can do this by showing $\exists x\in P, p(x)$, the existential theorem, is false
- Below is the brute force method
$$
\begin{align}
\lnot&(\exists x\in D, p(x)) && \text{is true} \\
\equiv&\forall x\in D, \lnot p(x) && \text{is true} \\
\equiv& \forall x\in D, Q(x)
\end{align}
$$
- Below is the generalizing method
	This can be combined with the [[Valid and Invalid Arguments#Special Cases|Division of Cases]] 
Let x be an arbitrary chosen element in D, then you want to show p(x) is true
```ad-example
$\forall x\in\mathbb{Z}, x(x+1)$ is even. Call this $p(x)$
Let x be an arbitrary element in $\mathbb{Z}$
#### Case 1: X is even
$$
\begin{align}
x=&2k, \\
x(x+1)=& 2k(2k+1) \\
=& 2(k(2k+1)) && \text{is even} \\
\end{align}
$$
#### Case 2: X is odd
```
