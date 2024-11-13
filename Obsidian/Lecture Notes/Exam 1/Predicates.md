>[!def] Predicate
>A predicate is a sentence that contains a finite number of variables, and becomes a statement when specific values are assigned.

>[!def] 
>If $p(x)$ is a predicate and x had domain D, the truth set of $p(x)$ is the set of all $x\in D$ that makes $p(x)$ a true statement.
>$\set{x\in D|p(x)}$

>[!def] Universal Statement
>for all/any $\forall$: for any universal qualifiers
>$\forall x\in D, p(x)$ is True if every $x\in D,p(x)$ is True.
#### $\forall x\in D,p(x)$ is *true* for any $x\in D,p(x)$ is a true statement. It is *false* if there exists $(\exists)$ at least one $x\in D$ such that $p(x)$ is false.
>[!ttheory] Fermat's Last Theorem
>$\forall x,y,z \in \mathbb{Z}$, and $n\ge 3$,
>$x^n +y^n = z^n$ has no solution.

>[!def] Existential Statement
>there exists $\exists$, there is existential qualifier
>$\exists\ x\in D, p(x)$
#### $\exists\ x\in D,p(x)$ is *true* if there exists $x\in D$, $p(x)$ is a true statement. It is *false* is for every $x\in D$, $p(x)$ is false.
>[!theory] Theorem 3: Negation of a Universal Qualifier
>$\lnot(\forall\ x\in D, p(x)) \equiv \exists\ x\in D, \lnot p(x)$

>[!def]
>Let $p(x)$ and $Q(x), p(x) \implies Q(x)$: If the truth set of $p(x)$ is a subset of truth set of $Q(x)$.
## Contrapositive, Converse, and Inverses
```ad-def
Consider the statement in the form $\forall x\in D$, if $P(x)$ then $Q(x)$
1. Its contrapositive is the statement: $\forall x\in D, \text{ if } \lnot Q(x)\text{ then } \lnot P(x)$
2. Its Converse is the statement $\forall x\in D, \text{ if } Q(x) \text{ then } P(x)$
3. Its inverse is the statement $\forall x \in D, \text{ if } \lnot P(x) \text{ then } \lnot Q(x)$
```
## Truth by default
>[!def] True by default
>Vacuous truth. $\forall x\in D, p(x)\to Q(x)$ is true by default if $\forall x\in D, p(x)$ is false.
#### Proof:
$$
\begin{align}
\forall x\in D, p(x)\to Q(x) \equiv& \forall x\in D, \lnot p(x)
\lor Q(x) \\
\equiv& \forall x\in D, t\lor Q(x) \\
\equiv& \forall x\in D, t
\end{align}
$$
```ad-example
Let $x$ be a abll, $D=\set{B,B,B,W,W,W}$.
$p(x)$ = ball $x$ in the bucket
$Q(x)$ = ball $x$ is B
$\forall x\in D, p(x)\to Q(x)$ All bucks in the bucket are B
If no balls in the bucket, $\forall x\in P, p(x)\to Q(x)$ is ALWAYS true
```
