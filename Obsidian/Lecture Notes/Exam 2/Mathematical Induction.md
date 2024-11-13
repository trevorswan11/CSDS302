#### Recall the Universal Statement
$$
\forall n\in\mathbb{Z}^+,n\ge a, p(n)
$$
## Steps to Proving with Induction
**Step 1 (Basic Step):** Show that $p(a)$ is true
**Step 2 (Inductive Step):** Show that for any integer $k\ge a$, if $p(k)$ is true, then $p(k+1)$ is also true
$$
\forall k\ge a, p(k)\to p(k+1)
$$
#### Example
Assume $\sum_\limits{i=1}^k i=\frac{k(k+1)}{2}$
Then try $k + 1$
$$
\begin{align}
\sum_\limits{i=1}^{k+1}i=& \frac{(k+1)(k+2)}{2} && \text{Is this true?}\\
\sum_\limits{i=1}^{k+1}i=& \sum_\limits{i=1}^k i +(k+1) \\
\text{by }p(k)=& \frac{k(k+1)}{2}+(k+1) \\
=& \frac{(k+1)(k+2)}{2} && \text{Yes, this is true }\checkmark
\end{align}
$$
Most important step here is that you're trying to determine $p(k+1)$ in terms of $p(k)$
#### Definitions
```ad-def
title: Arithmetic Sequence
Given $a,b\in\mathbb{R}$ and $k\in\mathbb{Z}$, k is fixed.
$$\set{a+bk}_{k\ge 0}$$ 
The above is an arithmetic sequence with common difference $b$
```
**These types of sequences have common *differences***
```ad-def
title: Geometric Sequence
$$\set{r^k}_{k\ge 0} = \set{1,r,r^2\dots}$$
```
**These types of sequences have common *ratios***
#### Theorem 5.2.3
```ad-theory
$$
\forall n\in\mathbb{Z},\sum_\limits{i=0}^n r^i=\frac{r^{n+1}-1}{r-1}\text{ with } r\neq1
$$
```
#### Pf/ a=0
**Step 1:** $p(0), \sum_\limits{i=0}^{0}r^i=r-\frac{r-1}{r-1}\checkmark$
**Step 2:** Assume $p(k)$ is true
$$
\begin{align}
\sum_\limits{i=0}^k r^i =& \frac{r^{n+1}-1}{r-1} \checkmark  \\
&\text{WTS (want to show) p(k+1) is true} \\
\sum_\limits{i=0}^{k+1} r^i =& \frac{r^{k+2}-1}{r-1} && \text{?} \\
\sum_\limits{i=0}^{k+1} r^i =& \sum_\limits{i=0}^k r^i + r^{k+1} && \star \\
=& \frac{r^{k+1}-1}{r-1} + r^{k+1} = \frac{r^{k+1}-1}{r-1} + \frac{r^{k+1}(r-1)}{r-1} \\
=& \frac{r^{k+1} - 1+r^{k+2} -r^{k+1}}{r-1} \\
=& \frac{r^{k+2}}{r-1} && \text{This is True} 
\end{align}
$$
## Limits of Mathematical Induction
*You need a **true conclusion** in order for it to work, which is sometimes very difficult to have*
(suggestion limit reached)
## More on Mathematical Induction
Prove the following:
$$
\forall n\in\mathbb{Z}, n\ge 0, 3|(2^{2n}-1)
$$
#### Pf/ a=0
**Step 1:** $p(0)\to3|0\ \checkmark$ 
**Step 2:** Assume $p(k)$ is true
$$
\begin{align}
3\mid&(2^{2k}-1) \\
\text{WTS: } 3\mid&(2^{2(k+1)}-1) \\
2^{2(k+1)}-1=&2^{2k+2}-1 \\
=& 4\cdot2^{2k}-1 && ?\\
=& 4(2^{2k}-1+1)-1 \\
=& 4(2^{2k})-1 \\
=& 4(2^{2k}) - 4 + 3 && \text{Rearrange} \\
=& 4(2^{2k}-1) +3 && \text{Simplify}
\end{align}
$$
Since $2^{2k}-1$ is divisible by three and 3 is also divisible by three, then $p(k)$ is divisible by 3.

## Mathematical Induction; Another Example
$$
\forall n\in\mathbb{Z},n\ge3\qquad2n+1<2n
$$
#### Pf/ a=3
**Step 1:** $p(3), 7<8\ \checkmark$
**Step 2:** Assume $2k+1<2^k$  is true
$$
\begin{align}
2k+1 <& 2^k \\
\text{WTS: } 2(k+1)+1<&2^{k+1} \\
2(k+1)+1=2k+3=&2k+1+2 \\
<& 2^k+2 < 2^k +2^k \\
=&2\cdot2^k  \\
=&2^{k+1}
\end{align}
$$
## Strong Mathematical Induction
*Very similar to the previous method, it just uses a different assumption*
$$
\forall n\in\mathbb{Z},n\ge 2 \qquad \text{n is divisible by a prime}
$$
#### Pf/ a=2 (Not Strong)
**Step 1:** $p(2), 2|2\ \checkmark$
**Step 2:** Assume k is divisible by a prime $p_1$
$$
\begin{align}
\text{WTS: } k+1&\dots \\
k=&p_1m \\
k+1=&p_1m+1\ / p_2
\end{align}
$$
Help step bro I'm stuck
#### Pf/ (Strong)
$$
\forall n\in\mathbb{Z}, n\ge a, p(n)
$$
**Step 1 (Basic Step):** $p(a)$ is true 
**Step 2:** Assume $\forall k\ge a$
$$
\set{p(a),p(a+1),\dots,p(k)}\to p(k+1)
$$
We can therefore say that $p(k)\to p(k+1)$
****
Assume k is divisible by a prime $p_1$, $\set{p(2),p(3),\dots,p(k)}$ all true 
*The above is called a reasonable assumption*
#### Case 1: $k+1$ is prime
$k+1|k+1$ DONE
#### Case 2: $k+1$ is not prime
$$
\begin{align}
k + 1 =& r\cdot s \\
1<r,s<&k+1 && \text{By the defintion of a composite Integer}
\end{align}
$$
$$
\begin{align}
p(r) \text{ is true by} &\text{ Strong MI Assumption} \\
p|r\to &p|k+1
\end{align}
$$
## Summary of Mathematical Induction
#### Mathematical Induction
$p(a)$ is true, $\forall k\ge a, p(k)\to p(k+1)$
#### Strong Mathematical Induction
$p(a)$ is true, $\forall k\ge a, \set{p(a),p(a+1)\dots p(k)}\to p(k+1)$
# Fundamental Theorem
```ad-theory
title: Theorem 5.4.1
$\forall n\in\mathbb{Z}^+, n$ has a $\underline{\underline{\text{unique}}}$ binary representation.
$n=C_r\cdot2^r+C_{r-1}\cdot2^{r-1}+\dots+C_2\cdot2^2+C_1\cdot2+C_0\cdot2^0$
```
#### Example
$$
100 = 2^6+2^5+2^2
$$
In binary, this can be represented as:
$$
\begin{align}
2^6+2^5+0\cdot2^4+0&\cdot2^3+2^2+0\cdot2+0 \\
1\ 1\ 0\ 0\ &1\ 0\ 0 
\end{align}
$$
```ad-example
title: Examples of Binary Representation
$$
5=1\cdot2^2+0\cdot2+1\cdot2^0 \to 1\ 0\ 1
$$
****
$$
4=1\cdot2^2+0\cdot2+0\cdot2^0 \to 1\ 0\ 0
$$
```
## Proof of the Fundamental Theorem
*Making use of strong mathematical induction*
## Step 1: Basis Step
$p(1)$ is true: $1=1\cdot2^0$
## Step 2: inductive Step
Assume $\set{p(1), p(2),\dots,p(k)}$ are all true.
WTS: $p(k+1)$ is true
#### Case 1: $k+1$ is even
$k+1=2\cdot\frac{K+1}{2}$
$$
\begin{align}
\frac{k+1}{2}=& 2^m + a_{m-1}2^{m-1}+\dots+a_12+a_02^0 \\
\text{Muliply by 2}=&2^{m+1}+a_{m-1}2^m+\dots+a_12^2+a_02 + 0\cdot2^0
\end{align}
$$
```ad-note
title: Doubling
Doubling a number is the same as adding an extra bit
$$\textbf{Number}\qquad\qquad\textbf{Binary}$$
$$4=2^2+0\cdot2+0\cdot2^0\to 1\ 0\ 0$$
$$8=2^3+0\cdot2^2+0\cdot2+0\cdot2^0\to 1\ 0\ 0\ 0$$
```
#### Case 2: $k+1$ is odd
$k+1=2\cdot\frac{k}{2}+1$
$$
\begin{align}
k+1=&2(2^m+\dots+a_02^0)+1 \\
=&2^{m+1}+a_{m-1}2^m+\dots+a_12^2+a_02+1
\end{align}
$$
## Proving the Theorem by Contradiction 
#### Uniqueness
Assume there exists $n\in\mathbb{Z}^+$ such that $n$ has two different binary representations.
**Two Different Representations**
$$
\begin{align} 
n=&2^m+a_{m-1}2^{m-1}+\dots+a_12+a_0 \\
=&2^k+b_{k-1}2^{k-1}+\dots+b_12+b_0
\end{align}
$$
$k\neq m$, Assume $k>m\text{ and } k\ge m+1$
$$
2^m+a_{m-1}2^{m-1}+\dots+a_12+a_02^0\le 2^m+2^{m-1}+\dots+2+2^0
$$
This is equal to 
$$
2^{m+1}-1\le2^k-1<2^k\le\underline{2^k+b_{k-1}2^{k-1}+b_12+b_0}\ (= n)
$$
This means that $n<n\to$ a contradiction! We can make this conclusion because the two comparisons of the values of n are not equal. 
$\square$

