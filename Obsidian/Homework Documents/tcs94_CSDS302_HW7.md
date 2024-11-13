# **CSDS302 HW7 - Trevor Swan (*tcs94*)**
# 6.1

## 1

In each of (b)–(d), answer the following questions: Is $A\subseteq B$? Is $B\subseteq A$? Is either $A$ or $B$ a proper subset of the other?

### b

$A=\{3,\sqrt{5^2-4^2},24\mod 7\}$
$B=\{8\mod 5\}$
```ad-answer
Simplifying the expressions seen in the sets reveals the following:
$$
\begin{align}
A=&\set{3, \sqrt{25-16}, 3}=\set{3, 3, 3} =\set{3}\\
B=&\set{3}
\end{align}
$$
Because repeated elements are treated as one element in sets, we can conclude that $\boxed{A=B}$.
```

### d

$A=\{a,b,c\}$
$B=\{\{a\},\{b\},\{c\}\}$
```ad-answer
Because $\set{a}\not\in A,\ \set{b}\not\in A,\ \set{c}\not\in A,\  A\not\subseteq B$ and $B\not\subseteq A$
```

## 4

$A=\{n\in\mathbf Z|n=5r,r\in\mathbf Z\}$
$B=\{m\in\mathbf Z|m=20s,s\in\mathbf Z\}$
Prove or disprove each of the following statements.

### a

$A\subseteq B$
```ad-answer
We can expand out the the two sets into the following set roster notation.
$$
\begin{align}
A=&\pm\set{5, 10, 15, 20, 25, 30, 35, \dots, 5r} \\
B=&\pm\set{20, 40, 60, \dots, 20s}
\end{align}
$$
For the statement, $A\subseteq B$ to be true, all elements in A must be elements in B. We can clearly see that there are elements in A that are not in B, so to disprove this statement we must provide a counterexample. Because $5\in A$ but $5\not\in B$, we ca conclude that the statement is false and $\boxed{A\not\subseteq B}$.
```

### b

$B\subseteq A$
```ad-answer
We can expand out the the two sets into the following set roster notation.
$$
\begin{align}
A=&\pm\set{5, 10, 15, 20, 25, 30, 35, \dots, 5r} \\
B=&\pm\set{20, 40, 60, \dots, 20s}
\end{align}
$$
For the statement, $B\subseteq A$ to be true, all elements in B must be elements in A. We can generalize A and say that A is the set of all integers divisible by 5. We can then say that B is the set of all integers divisible by 20, which therefore means its elements must all be divisible by both 5 and 4. Because an element in z is divisible by 5 where $z \mod 5 = 0$, then z is also an element in A, showing that the statement is true and $\boxed{B\subseteq A}$.
```

## 12

Let the universal set be $\mathbf R$, the set of all real numbers, and let
$A=\{x\in\mathbf R|-3\le x\le 0\}$
$B=\{x\in\mathbf R|-1<x<2\}$
$C=\{x\in\mathbf R|6<x\le8\}$
Find each of the following:

### a

$A\cup B$
```ad-answer
$$
\begin{align}
A\cup B=&\set{x\in\mathbb{R}|-3\le x\le0\text{ or }-1<x<2} \\
=&\set{x\in\mathbb{R}|-3\le x<2}
\end{align}
$$
```

### b

$A\cap B$
```ad-answer
$$
\begin{align}
A\cap B=&\set{x\in\mathbb{R}|-3\le x\le 0\text{ and }-1<x<2} \\ 
=&\set{x\in\mathbb{R}|-1,x\le 2}
\end{align}
$$
```

### g

$A^C\cap B^C$
```ad-answer
$$
\begin{align}
A^C\cap B^C=&\set{x\in\mathbb{R}|\lnot(-3\le x<0)\text{ and }\lnot(-1<x<2)} \\
=&\set{x\in\mathbb{R}|(x < -3\text{ or }x>0)\text{ and }(x\le-1\text{ or }x\ge 2)} \\
=&\set{x\in\mathbb{R}|x< -3\text{ and }x\ge 2}
\end{align}
$$
```

### i

$(A\cap B)^C$
```ad-answer
This statement can be broken down using De Morgan's law as follows:
$$
\begin{align}
(A\cap B)^C = A^C\cup B^C=&\set{x\in\mathbb{R}|\lnot(-3\le x<0)\text{ or }\lnot(-1<x<2)} \\
=&\set{x\in\mathbb{R}|(x < -3\text{ or }x>0)\text{ or }(x\le-1\text{ or }x\ge 2)} \\
=&\set{x\in\mathbb{R}|x\le-1\text{ or }x>0}
\end{align}
$$
```

## 25

$R_i=\left\{ x\in\mathbf R|1\le x\le 1+\frac{1}{i} \right\}=\left[ 1,1+\frac{1}{i} \right]\qquad:i\in\mathbf Z$

### a

$\bigcup\limits_{i=1}^4R_i=?$
```ad-answer
First we calculate the individual sets:
$$
\begin{align}
R_1=& \set{x\in\mathbb{R}|1\le x\le2} \\
R_2=& \set{x\in\mathbb{R}|1\le x\le\frac{3}{2}} \\
R_3=& \set{x\in\mathbb{R}|1\le x\le\frac{4}{3}} \\
R_4=& \set{x\in\mathbb{R}|1\le x\le\frac{5}{4}}
\end{align}
$$
Then we express these sets as a union:
$$
\begin{align}
\bigcup\limits_{i=1}^4R_i=&
\set{x\in\mathbb{R}|1\le x\le2}\cup
\set{x\in\mathbb{R}|1\le x\le\frac{3}{2}} \\
\cup&\set{x\in\mathbb{R}|1\le x\le\frac{4}{3}}
\cup\set{x\in\mathbb{R}|1\le x\le\frac{5}{4}}
\end{align}
$$
The Union must contain the elements in all of the sets, which can be shown as:
$$
\bigcup_{i=1}^4 R_i=\set{x\in\mathbb{R}|1\le x\le2}
$$
```

### c

Are $R_1,R_2,R_3,...$ mutually disjoint? Explain.
```ad-answer
For sets to be mutually disjoint, $R_1\cap R_2$ must be $\emptyset$. We see that:
$$
\begin{align}
R_1=& \set{x\in\mathbb{R}|1\le x\le2} \\
R_2=& \set{x\in\mathbb{R}|1\le x\le\frac{3}{2}}
\end{align}
$$
Where both $R_1$ and $R_2$ both contain the element 1, so they cannot be mutually disjoint.
```

### d

$\bigcup\limits_{i=1}^nR_i=?$
```ad-answer
First we calculate a few individual sets:
$$
\begin{align}
R_1=& \set{x\in\mathbb{R}|1\le x\le2} \\
R_2=& \set{x\in\mathbb{R}|1\le x\le\frac{3}{2}} \\
R_3=& \set{x\in\mathbb{R}|1\le x\le\frac{4}{3}} \\
R_4=& \set{x\in\mathbb{R}|1\le x\le\frac{5}{4}} \\
R_n=& \set{x\in\mathbb{R}|1\le x\le\frac{n+1}{n}}
\end{align}
$$
Then we express these sets as a union:
$$
\begin{align}
\bigcup\limits_{i=1}^4R_i=&
\set{x\in\mathbb{R}|1\le x\le2}\cup
\set{x\in\mathbb{R}|1\le x\le\frac{3}{2}} \\
\cup&\set{x\in\mathbb{R}|1\le x\le\frac{4}{3}}
\cup\dots\cup\set{x\in\mathbb{R}|1\le x\le\frac{n+1}{n}}
\end{align}
$$
We can see that $2>(\frac{n+1}{n})$ for $n\in\mathbb{Z}, n>1$, so we can say that the following is true:
$$
\bigcup_{i=1}^n R_i=\set{x\in\mathbb{R}|1\le x\le2}
$$
```

### f

$\bigcup\limits_{i=1}^\infty R_i=?$
```ad-answer
First we calculate a few individual sets:
$$
\begin{align}
R_1=& \set{x\in\mathbb{R}|1\le x\le2} \\
R_2=& \set{x\in\mathbb{R}|1\le x\le\frac{3}{2}} \\
R_3=& \set{x\in\mathbb{R}|1\le x\le\frac{4}{3}} \\
R_4=& \set{x\in\mathbb{R}|1\le x\le\frac{5}{4}} \\
\dots \\
R_n=& \set{x\in\mathbb{R}|1\le x\le\frac{n+1}{n}}
\end{align}
$$
Then we express these sets as a union:
$$
\begin{align}
\bigcup\limits_{i=1}^4R_i=&
\set{x\in\mathbb{R}|1\le x\le2}\cup
\set{x\in\mathbb{R}|1\le x\le\frac{3}{2}} \\
\cup&\set{x\in\mathbb{R}|1\le x\le\frac{4}{3}}
\cup\dots\cup\set{x\in\mathbb{R}|1\le x\le\frac{n+1}{n}}
\end{align}
$$
Then we take the limit as n goes to infinity:
$$
\begin{align}
\lim_\limits{n\to\infty}\bigcup\limits_{i=1}^nR_i=&
\set{x\in\mathbb{R}|1\le x\le2}\cup
\set{x\in\mathbb{R}|1\le x\le\frac{3}{2}} \\
\cup&\set{x\in\mathbb{R}|1\le x\le\frac{4}{3}}
\cup\dots\cup\set{x\in\mathbb{R}|1\le x\le\frac{n+1}{n}}
\end{align}
$$
We can determine long term behavior by looking at the last term in the Union:
$$
\lim_\limits{n\to\infty}\set{x\in\mathbb{R}|1\le x\le\frac{n+1}{n}}=\set{x\in\mathbb{R}|1\le x\le1}
$$
All possible values in the set are bounded by 1 and 2 as $2>(\frac{n+1}{n})$ for $n\in\mathbb{Z}, n>1$, so we can say:
$$
\bigcup_{i=1}^\infty R_i=\set{x\in\mathbb{R}|1\le x\le2}
$$
```

## 29

Let $\mathbf R$ be the set of all real numbers. Is $\{\mathbf R^+,\mathbf R^-,\{0\}\}$ a partition of $\mathbf R$? Explain your answer.
```ad-answer
Suppose we define a variable $x\in\mathbb{R}$. If $x$ is a non-zero number, then it is either positive or negative. This allows us to say:
$$
\begin{align}
\mathbb{R}^+\cup\mathbb{R}^-\cup\set{0}=&\mathbb{R} \\
\mathbb{R}^+\cap\mathbb{R}^-=&\set{0}
\end{align}
$$
We can clearly see that $\mathbb{R}^+\cap\set{0}=\mathbb{R}^-\cap\set{0}=\set{0}$. We can therefore conclude that $\{\mathbb R^+,\mathbb R^-,\{0\}\}$ is a partition of $\mathbb{R}$.
```

# 6.2

Use an element argument to prove each statement in 17–18. Assume that all sets are subsets of a universal set $\mathbf U$.

## 17

For all sets $A, B, C$, if $A\subseteq B$ then $A\cup C\subseteq B\cup C$.
```ad-answer
Let $x\in A\cup C$, which splits this into two cases by the definition of the union of two sets.
#### Case 1: $x\in A$
Since $x\in A$, then we can say $x\in B$ since $A\subseteq B$. Therefore it is true to say that $x\in B\text{ or }x\in C$, where we can then say that $x\in B\cup C$. Substituting x yields:
$$
A\cup C\subseteq B\cup C
$$
#### Case 2:
Since $x\in C$ we can say that $x\in B\text{ or }x\in C$, where we can then say that $x\in B\cup C$. Substituting x yields:
$$
A\cup C\subseteq B\cup C
$$
Both cases lead to the desired conclusion so we have proved that for all sets $A, B, C$, if $A\subseteq B$ then $A\cup C\subseteq B\cup C$.
```

## 18

For all sets $A$ and $B$, if $A\subseteq B$ then $B^C\subseteq A^C$
```ad-answer
Suppose A and B are sets where $A\subseteq B$. Let $x\in B^C$. To show that $B^C\subseteq A^C$ is true, we must show that $x\in A^C$ by the definition of a subset.
****
Since $x\in B^C,\text{ then }x\not\in B$. If $x\in A$, then it is implied that $x\in B$ because of the given condition where $a\subseteq B$. Because we have shown that $x\in B$ cannot be true, then we have also shown that $x\in A$ cannot be true either.
#### Conclusion
We can conclude that $x\not\in A$, which by the definition of a complement is $x\in A^C$. Since every element in $B^C$ is also an element of $A^C$, then $B^C\subseteq A^C$ by the definition of a subset.
```

## 25

Find the mistake in the following “proof” that for all sets $A$ and $B$, $(A-B)\cup(A\cap B)\subseteq A$

“Proof: Suppose $A$ and $B$ are any sets, and suppose $x\in(A-B)\cup(A\cap B)$. If $x\in A$ then $x\in A-B$ and so, by definition of difference, $x\in A$ and $x\not\in B$ In particular, $x\in A$, and, therefore $(A-B)\cup(A\cap B)\subseteq A$ by definition of subset.”
```ad-answer
It is incorrect to claim that if $x\in A$, then $x\in A-B$. The reverse of this is true, where if $x\in A-B$, then $x\in A$. To prove this statement correctly, one would have to individually prove that $A-B\subseteq A$ and $A\cap B\subseteq A$. This proof is not doen here because it was not asked of me.
```

## 42

For every positive integer $n$, if $A_1,A_2,A_3,...$ and $B$ are any sets, then

$\bigcap\limits_{i=1}^n(A_i-B)=\left(\bigcap\limits_{i=1}^nA_i\right)-B$
```ad-answer
I will prove the above by using mathematical induction.
****
#### Basis Step
Let $P(n)$ be $\bigcap\limits_{i=1}^n(A_i-B)=\left(\bigcap\limits_{i=1}^nA_i\right)-B$, for $n\in\mathbb{Z}, n\ge1$.
We first must show that $P(1)$ is true. So n=1:
$$
\begin{align}
\text{LHS:} && \bigcap\limits_{i=1}^n(A_i-B)=&\bigcap\limits_{i=1}^1(A_i-B)=A_1-B \\ 
\text{RHS:} && \left(\bigcap\limits_{i=1}^nA_i\right)-B=&\left(\bigcap\limits_{i=1}^1A_i\right)-B=A_1-B
\end{align}
$$
Both sides of the expression evaluate to the same thing, so n=1 is true.
#### Inductive step
Assume that $P(k)$ is true where $\bigcap\limits_{i=1}^k(A_i-B)=\left(\bigcap\limits_{i=1}^kA_i\right)-B$. We must show that $P(k+1)$ is true where $\bigcap\limits_{i=1}^{k+1}(A_i-B)=\left(\bigcap\limits_{i=1}^{k+1}A_i\right)-B$.
$$
\begin{align}
\bigcap\limits_{i=1}^{k+1}(A_i-B)=&\bigcap\limits_{i=1}^k(A_i-B)\cap(A_{k+1}-B) && \text{Split Intersection} \\
=&(\left(\bigcap\limits_{i=1}^kA_i\right)-B)\cap(A_{k+1}-B) && \text{Use }P(k) \\
\textit{Use }(A-B)&\cap(C-B)=(A\cap C)-B\textit{ to do next step} \\
=&\left(\left(\bigcap\limits_{i=1}^kA_i\right)\cap A_{k+1}\right)-B \\
=& \left(\bigcap\limits_{i=1}^{k+1}A_i\right)-B && \text{Simplify}
\end{align}
$$
Thus $P(k+1)$ is true and we can say that $\bigcap\limits_{i=1}^n(A_i-B)=\left(\bigcap\limits_{i=1}^nA_i\right)-B$, for $n\in\mathbb{Z}, n\ge1$ by mathematical induction.
$\square$
```

# 9.2

## 11

### c

How many bit strings of length $8$ begin and end with a $1$?
```ad-answer
Here, the first and last character in the string are fixed to be 1, so the remaining 6 possible bits can either be a 0 or a 1. We can determine the possible number of strings by:
$$
1\cdot2\cdot2\cdot2\cdot2\cdot2\cdot2\cdot1=2^6=\boxed{64}
$$
```

## 17

### c

How many integers from $1000$ through $9999$ have distinct digits?
```ad-answer
Since the numbers must be between 1000 and 9999, then the first digit cannot be zero and the rest of the digits cannot be repeats of previous ones. There are 10 digits from 0 to 9, which we must contend with. To calculate the total number of integers in this range with these specifications, we can represent the number of possibilities per slot as:
- First: 9 ways as 0 cannot be the first digit
- Second: 9 ways as 0 can be a digit but cannot be a repeat of 1.
- Third: 8 ways as it cannot be duplicate of the previous 2 slots.
- Fourth: 7 ways as this digit cannot be the same as the previous two.
Using the multiplication rule, we can say the total number is:
$$
9\times9\times8\times7=\boxed{4536}
$$
```

### e

What is the probability that a randomly chosen four-digit integer has distinct digits? has distinct digits and is odd?
```ad-answer
There are 9000 numbers with 4 digits. We know that there are 2240 possible odd digits with distinct digits between 1000 and 9999 inclusive. Thus we have the following two solutions:
$$
\begin{align}
P(\text{Distinct})=&\frac{4536}{9000}=\boxed{50.4\%} \\
P(\text{Distinct \& Odd})=&\frac{2240}{9000}\approx\boxed{24.89\%}
\end{align}
$$
```

## 21

Suppose $A$ is a set with $m$ elements and $B$ is a set
with $n$ elements.

### a

How many relations are there from $A$ to $B$? Explain.
```ad-answer
A relation between two sets is defined as a subset of the cartesian product of these two sets. We first must determine the number of elements in the cartesian product of the sets.
$$
A\times B=m\times n=mn
$$
There are two ways to arrange each of the possitions in the product, one where the first element is from set A, and the other where the second element is from set A. We can then use the multiplication rule where we multiply 2 times itself $mn$ times.
$$
2\times2\times2\dots\times2=2^{mn}
$$
Therefore we can say there are $2^{mn}$ possible relations.
```

### b

How many functions are there from $A$ to $B$? Explain.
```ad-answer
Since there are $n$ elements in B, there are are only $n$ options for each element in A since a function must have exactly one image per element. We can use the multiplication rule to multiply n by itself m times.
$$
n\times n\times n\dots\times n=n^m
$$
Therefore we can say that there are $n^m$ possible functions from A to B.
```

### c

What fraction of the relations from $A$ to $B$ are functions?
```ad-answer
Using the results of parts a and b, the fraction of relations that are also functions is:
$$
\frac{n^m}{2^{mn}}
$$
```

## 31

### d

If $p_1,p_2,...,p_m$ are distinct prime numbers and $a_1,a_2,...,a_m$ are positive integers, how many distinct positive divisors does $p_1^{a_1}p_2^{a_2}...p_m^{a_m}$ have?
```ad-answer
We know by the way powers work, $p_1^{a_1}$ has $a_1 + 1$ positive divisors. We can then, by extension, say that $p_1^{a_m}$ has $a_m + 1$ positive divisors. Because we know $p$ is a distinct prime number, we can say:
- $p_1^{a_1}$: Has $a_1+1$ ways
- $p_2^{a_2}$: Has $a_2+1$ ways
- $\dots$
- $p_m^{a_m}$: Has $a_m+1$ ways
****
Using the multiplication we can conclude that the total number of distint positive divisors of the product $p_1^{a_1}p_2^{a_2}...p_m^{a_m}$ is:
$$
(a_1+1)(a_2+1)\dots(a_m+1)
$$
```

### e

What is the smallest positive integer with exactly $12$ divisors?
```ad-answer
First we will split 12 into its factors:
$$
12 = 3\cdot2\cdot2=4\cdot3=6\cdot2
$$
We can then use these factorizations to respresent cases with the three smallest prime numbers:
- Case One: $(a_1+1)(a_2+1)(a_3+1)= 3\cdot2\cdot2$
	- $a_1=2, a_2=1, a_3=1$
	- $2^23^15^1=60$
- Case Two: $(a_1+1)(a_2+1)= 4\cdot 3$
	- $a_1=3, a_2=2$
	- $2^33^2=72$
- Case Three: $(a_1+1)(a_2+1)= 6\cdot2$
	- $a_1=5, a_2=1$
	- $2^53=96$
****
Of these three cases, the smallest number is 60, showing that the smallest positive number with exactly 12 divisors is $\boxed{60}$.
```

## 39

### b

How many ways can six of the letters of the word $ALGORITHM$ be selected and written in a row?
```ad-answer
$$
P(n,r)=\frac{n!}{(n-r)!}
$$
We are selecting 6 of the 9 letters, so $n=9$ and $r=6$:
$$
P(7,4)=\frac{9!}{(9-6)!}=60480
$$
```

### d

How many ways can six of the letters of the word $ALGORITHM$ be selected and written in a row if the first two letters must be $OR$?
```ad-answer
$$
P(n,r)=\frac{n!}{(n-r)!}
$$
We are selecting 4 of the 7 letters, so $n=7$ and $r=4$. This is because the first two letters must be $OR$, so we reduce our values by 2 with respect to previous parts:
$$
P(7,4)=\frac{7!}{(7-4)!}=840
$$
```

# 9.3

## 2

### b

How many strings of hexadecimal digits consist of from two through five digits?
```ad-answer
Let's define the following 5 sets where $A=A_1+A_2+A_3+A_4$ by the addition rule:
- $A$= Strings of 2 to 5
- $A-1$= Strings of 2
- $A_2$=Strings of 3
- $A-3$= Strings of 4
- $A_4$=Strings of 5
****
We can then find the total number in each set:
- $N(A_1)=16\times16=256$
- $N(A_2)=16\times16\times16=4096$
- $N(A_3)=16\times16\times16\times16=65536$
- $N(A_4)=16\times16\times16\times16\times16=1048576$
****
The sum of these is the total number of strings:
$$
256+4096+65536+1048576=\boxed{1118464}
$$
```

## 7

At a certain company, passwords must be from 3–5 symbols long and composed from the 26 uppercase letters of the Roman alphabet, the ten digits 0–9, and the 14 symbols !, @, #, $, %, ^, &, \*, (, ), 2, 1, {, and }.

### c

How many passwords have at least one repeated symbol?
```ad-answer
There are 50 possible options for each slot of the password, with there being 3 differnt length options, we can say that:
$$
50^3+50^4+50^5=318875000
$$
Thus there are 31887500 total combinations.
We can then compute the possible number of passwords without a repeat of a symbol:
$$
(50\times49\times48)+(50\times49\times48\times47)+(50\times49\times48\times47\times46)= 259896000
$$
Subtracting the total number of combinations from those that dont have repetition yields:
$$
318875000-259896000=\boxed{58979000}
$$
```

### d

What is the probability that a password chosen at random has at least one repeated symbol?
```ad-answer
This probability can be determined by dividing the total number of passwords with a repeated symbol by the total number of possible passwords:
$$
\frac{5567900}{58979000}\approx0.18496=\boxed{18.296\%}
$$
```

## 17

### a

How many strings of four hexadecimal digits do not have any repeated digits?
```ad-answer
There are 16 possible hexadecimal characters. This calculation can be thought of as no replacement as follows:
$$
16\times15\times14\times13=\boxed{43680}
$$
```

### b

How many strings of four hexadecimal digits have at least one repeated digit?
```ad-answer
First we must determine the number of total hexadecimal strings with no restrictions:
$$
16^4=65536
$$
The total number of strings with at least one repeated digit is the difference between the total number and the amount with repeated digits:
$$
65536-43680=\boxed{21856}
$$
```

### c

What is the probability that a randomly chosen string of four hexadecimal digits has at least one repeated digit?
```ad-answer
The probability that a randomly chosen string has at least one repeated digit can be calculated by determining the fraction of strings with at least one repeated digit:
$$
\frac{21856}{65536}\approx0.3335=\boxed{33.35\%}
$$
```

## 23

### b

Suppose an integer from $1$ through $1000$ is chosen at random. Find the probability that the integer is a multiple of 4 or a multiple of 7.
```ad-answer
#### Total Integers that are a multiple of 4:
- $4=4\cdot1$
- $8=4\cdot2$
- $12=4\cdot3$
- $\dots$
- $1000=4\cdot 250$
Therefore there are 250 multiples of 4 from 1 to 1000.
#### Total Integers that are a multiple of 7:
- $7=7\cdot1$
- $14=7\cdot2$
- $21=7\cdot3$
- $\dots$
- $994=7\cdot142$
Therefore there are 142 multiples of 7 from 1 to 1000.
#### Total Integers that are a multiple of 28 (both 7 and 4):
- $28=28\cdot1$
- $56=28\cdot2$
- $84=28\cdot3$
- $\dots$
- $980=28\cdot35$
Therefore there are 980 multiples of 28 from 1 to 1000.
****
Thus the total number of integers divisible by 4 or 7 is:
$$
250+142-35 = 357
$$
*We had to subtract overlap to calculate correctly.*
Therefore the probability that a randomly selected integer from 1 to 1000 is divisible by either 4 or 7 is:
$$
\frac{357}{1000}=0.357=\boxed{35.7\%}
$$
```

### c

How many integers from $1$ through $1000$ are neither multiples of $4$ nor multiples of $7$?
```ad-answer
If we define the integers that are divisble by 4 as set A and those divisible by 7 as set B, then the integers divisible by neither 4 nor 7 is $(A\cup B)^C$:
$$
(A\cup B)^C=1000-357=\boxed{643}
$$
```

#### Thank you to Trevor Nichols for copying textbook questions into a markdown format 