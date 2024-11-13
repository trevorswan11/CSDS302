# Subsets and Equality
## Universal Statement
$$
A\subseteq B, \text{ if }\forall x\in A, x\in B
$$
$A\subset B$,, a proper subset if both:
$$
A\subseteq B, \text{ and }A\neq B
$$
#### Example
$$
\begin{align}
A=&\set{n\in\mathbb{Z}|n=10m-25\text{ for }m\in\mathbb{Z}} \\
B=&\set{n\in\mathbb{Z}|b=5r\text{ for }r\in\mathbb{Z}}
\end{align}
$$
```ad-example
title:Proper Subset Proof
#### Part 1
$$A\subseteq B$$
Let $x\in A$
$$
x = 10m-25=5(2m-5)\in B
$$
True as $2m-5\in\mathbb{Z}$
$\therefore A\subseteq B$
#### Part 2
$$A\neq B$$
Let $x = 10$
$$
x = 10=5\times2\in B\not \in A
$$
$\therefore A\neq B$
```
#### Example
$$
\begin{align}
A =&\set{n\in\mathbb{Z}|n=5m-25} \\
B=&\set{n\in\mathbb{Z}|b=5r}
\end{align}
$$
```ad-example
title:Equality of Sets
$$
A=B \text{ if }A\subseteq B\text{ and }B\subseteq A
$$
#### Part 1
Let $x = 5r$
$$
x = 5r= 5r+25-25=5(r+5)-25\in A
$$
Conclusion exactly the same as above example,
#### Part 2
Let $x\in B:x=5r$
$$
x=5r=5r+25-25\dots
$$
Same conclusion as above.
$\square$
```
# Operations with Sets
Let A and B be sets, where $U$ is the Universal Set
```ad-def
title: Set Notations
#### Union
$A\cup B = \set{x\in U|x\in A \textbf{ or }x\in B}$
![[Union]]
#### Intersection
$A\cap B = \set{x\in U|x\in A\textbf{ and }x\in B}$
![[Intersection]]
#### Difference
$A-B=\set{x\in U|x\in A\text{ and } x\not \in B}$
![[Difference]]
#### Complement
$A^c=\set{x\in U|x\not \in A}$
![[Complement]]
```
#### Example
For each $i\in\mathbb{Z}^+, i=1,2\dots$
Define $A_i=\left( -\frac{1}{i}, \frac{1}{i} \right)$ interval
	$A_1=(-1,1), A_2=\left( -\frac{1}{2}, \frac{1}{2} \right)$
```ad-example
title: Show that $A_{i+1}\subset A_i$
#### Part 1
$A_{i+1}\subseteq A_i$
Let $x\in A_{i+1}, x\in (-\frac{1}{i+1}, \frac{1}{i+1})$
$$
-\frac{1}{i}<x<-\frac{1}{i+1}<x<\frac{1}{i+1}<\frac{1}{i}
$$
$\therefore -\frac{1}{i}<x<\frac{1}{i}$
We can then conclude $x\in A_i$
#### Part 2
$A_{i+1}\neq A_i$
Any $x\in(\frac{1}{i+1}, \frac{1}{i})$
$\therefore x\in A_i$, but $x\not \in A_{i+1}$
```
#### 'Summation Notation'
**Union**
$$
\bigcup_{i=1}^{\infty} A_i = A_1\cup A_2\cup\dots\cup A_i
$$
**Intersection**
$$
\bigcap_{i=1}^{\infty} A_i = A_{\infty} = \set0
$$
#### Disjoint Sets
if $A\cap B =\emptyset$ then **disjoint**
Let $A_1,A_2,\dots A_n$
if $A_i\cap A_n=\emptyset$ then **Mutually Disjoint**
#### Partition of Set A
$$
\set{A_1, A_2\dots A_n}\text{ is a partition of A if:}
$$
1. $\bigcup_{i=1}^n A_i =A$
2. They are mutually disjoint