# **CSDS302 HW6 - Trevor Swan (*tcs94*)**
# 5.2

## 3

For each positive integer $n$, let $P(n)$ be the formula

$1^2+2^2+...+n^2= \frac{n(n+1)(2n+1)}{6}$

### a

Write $P(1)$. Is $P(1)$ true?
```ad-answer
The expression given can be written as the following;
$$1^2+2^2+\dots+n^2=\sum_\limits{i=1}^n i^2 = \frac{n(n+1)(2n+1)}{6}$$
****
- Therefore $P(1) = \sum_\limits{i=1}^1 i^2 = 1\leftarrow$ LHS
- The expression given evaluated for $P(1) = \frac{1(1+1)(21+1)}{6} = \frac{6}{6} = 1 \leftarrow$ RHS
****
The two results, or sides of the equation, are equal so $\boxed{P(1)\text{ is true}}$.
```

### b

Write $P(k)$
```ad-answer
Generating this expression is as simple as substituting $k$ for $n$ in the given formula.
$$\boxed{1^2+2^2+\dots+k^2=\frac{k(k+1)(2k+1)}{6}}$$
```

### c

Write $P(k+1)$
```ad-answer
Generating this expression involves substituting $k+1$ in the formula given for every instance of the variable $n$.
$$
\begin{align}
1^2+2^2+\dots+(k+1)^2=& \frac{(k+1)((k+1)+1)(2(k+1)+1)}{6} \\ 
=& \boxed{\frac{(k+1)(k+2)(2k+3)}{6}}
\end{align}
$$
```

### d

In a proof by mathematical induction that the formula holds for every integer $n\ge 1$, what must be shown in the inductive step?
```ad-answer
The inductive step must show that if $P(k)$ is true, then $P(k+1)$ is also true.
****
This would involve assuming $1^2+2^2+\dots+k^2=\frac{k(k+1)(2k+1)}{6}$ is true and then using that statement to prove that \frac{(k+1)(k+2)(2k+3)}{6} is also true. The second statement is $P(k+1)$.
```

## 7

Prove the statement using mathematical induction. Do not derive them from theorem 5.2.1 or theorem 5.2.2.

For every integer $n\ge1$
$1+6+11+16+...+(5n-4)= \frac{n(5n-3)}{2}$
```ad-answer
#### Step 1: $a=1\to P(1)=1=\frac{1(5(1)-3)}{2}$
This expression can be simplified to $1=1$ which is true $\checkmark$
#### Step 2: Assume $P(k)$ is true
$$
\begin{align}
\text{Assume } 1+6+11+16+...+(5k-4)=& \frac{k(5k-3)}{2} \text{ is true}&&\checkmark \\
\text{WTS: } 1+6+11+16+...+(5(k+1)-4)=& \frac{(k+1)(5(k+1)-3)}{2} && ? \\
1+6+11+16+...+(5k-4)+(5k+1)=& \frac{(k+1)(5k+2)}{2} \\
\text{Substitute Assumed: }\frac{k(5k-3)}{2}+(5k+1)=& \frac{(k+1)(5k+2)}{2} \\
\text{Rewrite: }\frac{k(5k-3)}{2} + \frac{2(5k+1)}{2}=& \frac{(k+1)(5k+2)}{2} \\
\text{Expand Terms: }\frac{5k^2-3k}{2} + \frac{10k+2}{2}=& \frac{(k+1)(5k+2)}{2} \\
\text{Simplify: }\frac{5k^2+7k+2}{2} =& \frac{(k+1)(5k+2)}{2} \\
\frac{(k+1)(5k+2)}{2} =& \frac{(k+1)(5k+2)}{2} && \checkmark
\end{align} 
$$
****
Because the two sides of the proof are equal, we can say that for every integer $n\ge 1$, $1+6+11+16+...+(5n-4)= \frac{n(5n-3)}{2}$ is true by mathematical induction. 
$\square$
```

## 12

Prove the statement using mathematical induction.

$\frac{1}{1\cdot 2}+\frac{1}{2\cdot 3}+...+\frac{1}{n(n+1)}=\frac{n}{n+1}$ for every integer $n\ge 1$
```ad-answer
#### Step 1: $a = 1\to P(1)=\frac{1}{1\cdot2}=\frac{1}{1+1}$
This expression can be simplified to $\frac{1}{2}=\frac{1}{2}$ which is true $\checkmark$
#### Step 2: Assume $P(k)$ is true
This assumption means that $\frac{k}{k+1}$ is true.
$$
\begin{align}
\text{RHS: }&\frac{1}{n(n+1)}= \frac{n}{n+1}\mid_{(k+1)} = \frac{k+1}{(k+1)+1} = \frac{k+1}{k+2} \\
\text{WTS: }&\frac{1}{1\cdot 2}+\frac{1}{2\cdot 3}+...+\frac{1}{(k+1)((k+1)+1)}\equiv \frac{k+1}{k+2} \\
\end{align}
$$
****
Below I will refer to $\frac{1}{1\cdot 2}+\frac{1}{2\cdot 3}+...+\frac{1}{(k+1)((k+1)+1)}$ as 'LHS'
$$
\begin{align}
\text{LHS}=& \frac{1}{1\cdot 2}+\frac{1}{2\cdot 3}+...+\frac{1}{(k+1)(k+2)} \\
=& \frac{1}{1\cdot 2}+\frac{1}{2\cdot 3}+...+\frac{1}{k(k+1)}+\frac{1}{(k+1)(k+2)} \\
\text{Use Assumption: }=& \frac{k}{k+1} + \frac{1}{(k+1)(k+2)} \\
\text{Rewrite: }=&\frac{k(k+2)}{(k+1)(k+2)} + \frac{1}{(k+1)(k+2)} \\
\text{Simplify: }=&\frac{k(k+2)+1}{(k+1)(k+2)} \\
=& \frac{k^2+2k+1}{(k+1)(k+2)} \\
=& \frac{(k+1)^2}{(k+1)(k+2)} \\
=& \frac{k+1}{k+2}
\end{align}
$$
****
The expression derived above is equivalent to the substitution of $k+1$ in the statement that is assumed to be true. Becuase these statements are equal, we can say that $\frac{1}{1\cdot 2}+\frac{1}{2\cdot 3}+...+\frac{1}{n(n+1)}=\frac{n}{n+1}$ for every integer $n\ge 1$ is true through mathematical induction.
$\square$
```

## 29

Use the formula for the sum of the first $n$ integers and/or the formula for the sum of a geometric sequence to evaluate the sum or to write it in closed form.

$1-2+2^2-2^3+...+(-1)^n2^n$ where $n$ is any positive integer
```ad-answer
To start we can rewrite the expression in terms of powers of negative two.
$$1-2+2^2-2^3+...+(-1)^n2^n\equiv(-2)^0+(-2)^1+(-2)^2+(-2)^3+\dots+(-2)^2$$
Therefore we can derive the following conclusion:
$$
\begin{align}
1-2+2^2-2^3+...+(-1)^n2^n =& (-2)^0+(-2)^1+(-2)^2+(-2)^3+\dots+(-2)^2 \\
=& \sum_\limits{i=0}^n (-2)^n \\
\textit{Theorem 5.2.3:}&\sum_\limits{i=0}^n r^i=\frac{r^{n+1}-1}{r-1} \\
\therefore\quad=& \frac{(-2)^{n+1}-1}{(-2)-1} \\
=&\frac{(-1)^{n+1}2^{n+1}-1}{-3} \quad\leftarrow\text{Exponent Rules} \\
=&\frac{1-(-1)^{n+1}2^{n+1}}{3} \quad\leftarrow\text{Simplify Negatives}
\end{align}
$$
$\therefore$ The sum of the given formula is $\boxed{\frac{1-(-1)^{n+1}2^{n+1}}{3}}$
```

# 5.3

## 4

For each positive integer $n$, let $P(n)$ be the sentence that describes the following divisibility property:

$5^n-1$ is divisible by $4$.

### a

Write $P(0)$. Is $P(0)$ true?
```ad-answer
$$P(0)=5^0-1=1-1=0$$
0 is divisible by any integer, and the conclusion can be written as:
$4|0$. Therefore the given statement evaluated at 0, $P(0)$ is true.
```

### b

Write $P(k)$
```ad-answer
This statement can be derived by substituting $k$ in for $n$
$$P(k)=5^k-1\text{ is divisble by 4}$$
```

### c

Write $P(k+1)$
```ad-answer
This statement can be derived by substituting $(k+1)$ in for $n$
$$P(k)=5^{k+1}-1\text{ is divisble by 4}$$
```

### d

In a proof by mathematical induction that this divisibility property holds for every integer $n\ge0$, what must be shown in the inductive step?
```ad-answer
The inductive step must show that $P(k+1)$ is true based on the assumption that $P(k)$ is true.
```

## 7

For each positive integer n, let P(n) be the sentence

In any round-robin tournament involving $n$ teams, the teams can be labeled $T_1,T_2,T_3,...,T_n$, so that $T_i$ beats $T_{i+1}$ for every $i=1,2,...,n$.

### a

Write $P(2)$. Is $P(2)$ true?
```ad-answer
In any round-robin tournament involving 2 teams, the teams can be labeled $T_1,T_2$, so that $T_2$ beats $T_3$.
```

### b

Write $P(k)$.
```ad-answer
In any round-robin tournament involving $k$ teams, the teams can be labeled $T_1, T_2, T_3,\dots,T_k$, so that $T_k$ beats $T_{k+1}$ for every $i=1,2,\dots,k$.
```

### c

Write $P(k+1)$
```ad-answer
In any round-robin tournament involving $k+1$ teams, the teams can be labeled $T_1,T_2,T_3,\dots,T_{k+1}$, so that $T_{k+1}$ beats $T_{k+2}$ for $i=1,2,\dots,k+1$.
```

### d

In a proof by mathematical induction that $P(n)$ is true for each integer $n\ge2$, what must be shown in the inductive step?
```ad-answer
To prove this using mathematical induction, we would have to show that in any round-robin tournament involving $k+1$ teams, the teams can be labeled $T_1,T_2,T_3,\dots,T_{k+1}$, so that $T_{k+1}$ beats $T_{k+2}$ for $i=1,2,\dots,k+1$. This would have to be proved for all integers $k$ such that $k\ge2$, in any round-robin tournament involving $k$ teams, the teams can be labeled $T_1, T_2, T_3,\dots,T_k$, so that $T_k$ beats $T_{k+1}$ for every $i=1,2,\dots,k$.
```

## 15

Prove the statement by mathematical induction

$n(n^2+5)$ is divisible by $6$, for each integer $n\ge0$
```ad-answer
#### Step 1: $a=0\to6|0(0^2+5)=6|0\quad\checkmark$
0 is divisible by any number, so $6|0$ is true.
#### Step 2: Assume $P(k)$ is true.
This means $P(k)=6\mid k(k^2+5)$ is true.
By the definition of divisibility, this means there exists an integer $m$ such that $k(k^2+5)=6m$. We will assume the previous expression is true.
****
$$\text{WTS: } (k+1)((k+1)^2+5)=6m\text{ for some integer m}$$
****
$$
\begin{align}
(k+1)((k+1)^2+5)=& (k+1)(k^2+2k+1+5) \\
=& (k+1)(k^2+2k+6) && \text{Combine Terms} \\
=& k^3 +2k^2 +6k +k^2+2k+6 && \text{Distribute} \\
=& k^3+3k^2+8k+6 && \text{Combine Terms} \\
=& k^3+5k+3k^2+3k+6 && \text{Break up Terms} \\
=& k(k^2+5)+3k^2+3k+6 && \text{Split first terms} \\
=& 6m+3k^2+3k+6 && \text{Substitute Given} \\
=& 6m+3k(k+1)+6 && \text{Break up Terms} \\
\star_1=& 6m +3(2l)+6 && \text{For some integer }l \\
=& 6m +6l +6 &&\text{Multiply} \\
=& 6(m+l+6) && \text{Factor out 6} \\
\end{align}
$$
$$\star_1:k\text{ and }k+1\text{are consecutive so one must be even with a product } 2l$$
$6(m+l+1)$ is divisibe by 6 because $m+l+1$ is an integer so $6|6(m+l+1)\to 6(m+l+1)=6q$ where $q=m+l+1$, an integer. This is done through the definition of divisibility, proving that $P(k+1)$ is divisible by 6.
****
Therefore, through mathematical induction, we can say that $n(n^2+5)$ is divisible by 6 for each integer $n\ge0$.
$\square$
```

# 5.4

## 10

The introductory example solved with ordinary mathematical induction in Section 5.3 can also be solved using strong mathematical induction. Let $P(n)$ be “any n¢ can be obtained using a combination of 3¢ and 5¢ coins.” Use strong mathematical induction to prove that $P(n)$ is true for every integer $n\ge8$.
```ad-answer
#### Step 1: Basis Step
Show $P(14), P(15),\text{ and },P(16)$ are true
$$
\begin{align}
P(14):& 14=3a+5b&&\text{True when }a=3,b=1&&\checkmark \\
P(15):& 15=3a+5b&&\text{True when }a=0,b=5&&\checkmark \\
P(16):& 16=3a+5b&&\text{Truw when }a=2,b=2&&\checkmark \\
\end{align}
$$
#### Step 2: Inductive Step
*Show that for every integer $k\ge 16$, if $P(i)$ is true for each integer from 16 through $k$, then $P(k+1)$ is also true.*
****
**Inductive Hypothesis:** Any $i\textcent$ can be obtained using a combination of $3\textcent$ and $5\textcent$ coins for all integers $i\ge 16$.
**$P(k+1)$:** We must show that any $(k+1)\textcent$ can be obtained using a combination of $3\textcent$ and $5\textcent$ coins.
****
Since $k\ge 16$, $k-2\ge14$ and $P(14)$ is true from earlier. This means $P(k-2)$ is true from the basis step. This means there are two positive integers $a$ and $b$ where $5a+3b=k-2$ is true.
We want to prove $k+1$ is true, so we will add 3 to each side of the equation.
$$
\begin{align}
5a+3b=&k-2 && \text{True} \\
5a+3b+3 =&k-2+3 && \text{Add 3 to each side} \\
5a+3(b+1)=&k+1 && \text{Combine terms} \\
5a+3c=&k+1 && \text{For some integer c}
\end{align}
$$
****
Becuase $b$ is an integer, $b+1$ is also an integer. This means that $(k+1)\textcent$ can be written as a sum of $5\textcent$ and $3\textcent$ coins. By strong mathematical induction, we can thus say that "Any $n\textcent$ can be obtained using a combination of $3\textcent$ and $5\textcent$ coins."
```

## 13

Use strong mathematical induction to prove the existence part of the unique factorization of integers theorem (Theorem 4.4.5). In other words, prove that every integer greater than $1$ is either a prime number or a product of prime numbers.
```ad-answer
#### Step 1: Basis Step
Show that $P(2)$ is true:
2 is either prime or a product of prime numbers.
$$
P(2): n=2;\text{ 2 is prime so the given sentence is true.}
$$
#### Step 2: Inductive Step
*Show that for every integer $k\ge2$, if $P(i)$ is true for each integer from 2 through $k$, then $P(k+1)$ is also true.*
****
**Inductive Hypothesis:** Any integer $i$ is either prime or a product of prime numbers if $2\le i<k$.
$P(k+1)$: We must show that any integer $k+1$ is either prime or a product of prime numbers.
****
##### Case 1: $k+1$ is prime
$k+1$ is prime in this case so the given property holds true.
##### Case 2: $k+1$ is not prime
$k+1$ is not prime, so it is composite. Composite numbers can be writen as $k+1=a\cdot b$, for $1<a,b<k+1$ by definition.
$a\text{ or }b\neq1$ because $k+1$ is not a prime number in this case.
We will assume the inductive hypothesis is true, so $a$ and $b$ can be written as a product of prime numbers as follows:
$$
\begin{align}
a=&(p_1\cdot p_2\cdot p_3\dots p_i) \\
b=&(q_1\cdot q_2\cdot q_3\dots q_j) \\
\end{align}
$$
For some integers $i,j$ and primes $p_i, q_j$.
****
Therefore $k+1=a\cdot b= (p_1\cdot p_2\cdot p_3\dots p_i)\cdot(q_1\cdot q_2\cdot q_3\dots q_j)$ is also a product of prime numbers. By strong mathematical induction, we can say that every integer greater than 1 is either a prime number or a product of prime numbers.
```

## 16

Use strong mathematical induction to prove that for every integer $n\ge2$, if $n$ is even, then any sum of $n$ odd integers is even, and if $n$ is odd, then any sum of $n$ odd integers is odd.
```ad-answer
#### Step 1: Basis Step
Show that the statement is true for $P(2),\text{ and }P(3)$.
$$
\begin{align}
\text{For integers }q,r,s\text{ and the definition}&\text{ of even and odd:} \\
P(2): (2q+1)+(2r+1) =& 2q+2r+2=2(q+r+1) &&\text{Even}\\
P(3): (2q+1)+(2r+1)+(2s+1)=&2q+2r+2s+2+1 \\
=&2(q+r+s+1)+1&&\text{Odd}
\end{align}
$$
These two cases show that the statement holds true here.
#### Step 2: Inductive Step
*Show that for every integer $k\ge2$, if $P(i)$ is true for each integer from 2 through $k$, then $P(k+1)$ is also true.*
****
**Inductive Hypothesis:** For every integer $i\ge2$,if $i$ is even, then any sum of $i$ odd integers is even, and if $i$ is odd, then any sum of $i$ odd integers is odd. 
$P(k+1)$: We must show that the statement is true for some integer $k+1$
****
##### Case 1: $k+1$ is even
We can set up a summation to represent the sum of $k+1$ odd integers.
Becasue $k+1$ is even, we can define an integer $n$ where $2n=k+1$ by the definition of an even number.
$$
\begin{align}
\sum_\limits{i=1}^{2n} (2i+1) =& (2\cdot 1+1)+(2\cdot 2+1)+\dots+(2(2n)+1) \\
=& 2(1+2+3+\dots+2n)+2n \\
=& 2(1+2+3+\dots+i)+2n \quad\text{Let }i=2n\\ 
\end{align}
$$
Because $i$ is even, we can use the inductive hypothesis to say that the first $i$ odd integers is sum is even.
$$
2(1+2+3+\dots+i)+i=2a+i
$$
This is true for some integer a. The sum of even integers is even, so we can say that the sum of an even number of odd integers is even.
##### Case 2: $k+1$ is odd
We can set up a summation to represent the sum of $k+1$ odd integers. Because $k+1$ is odd, we can define an integer $m$ where $2m+1=k+1$ by the definition of an odd number.
$$
\begin{align}
\sum_\limits{i=1}^{2m+1} (2i+1) =& (2\cdot1+1)+(2\cdot2+1)+\dots+(2(2m+1)+1) \\
=& 2(1+2+3+\dots+(2m+1))+(2m+1) \\
=& 2(1+2+3+\dots+i)+(2m+1) \quad\text{Let }i=2m+1\\
\end{align}
$$
Because $i$ is odd, we can use the inductive hypothesis to say that the first $i$ odd integers sum is odd.
$$
2(1+2+3+\dots)+2m+1=2b+i
$$
This is true for some integer b. The sum of an even integer and an odd integer is always odd, so we can say that the sum of $i$ odd integers is odd.
****
The two cases presented lead to a true conclusion with respect to the assumption and $k+1$. This allows us to conclude that for every integer $n\ge2$, if $n$ is even, then any sum of $n$ odd integers is even, and if $n$ is odd, then any sum of $n$ odd integers is odd.
```

## 17

Compute $4^1,4^2,4^3,4^4,4^5,4^6,4^7,4^8$. Make a conjecture about the units digit of $4^n$ where $n$ is a positive integer. Use strong mathematical induction to prove your conjecture.
```ad-answer
### Computation
$$
\begin{align}
4^1=& 4 \\
4^2=& 16 \\
4^3=& 64 \\
4^4=& 256 \\
4^5=& 1024 \\
4^6=& 4096 \\
4^7=& 16384 \\
4^8=& 65536
\end{align}
$$
### Conjecture
The units digit of $4^n$ for some positive integer $n$ is 4 when $n$ is odd and 6 when $n$ is even.
### Proof
Let $P(n)$ be the statement, if $n$ is odd, then $4^n$ has a units digit of 4, and the units digit is 6 is $n$ is even.
#### Step 1: Basis Step
Using the computation above, we can see that $P(1):4^1=4$, when $n=1$, an odd number. Therefore $P(1)$ is true. We can also see that $P(2):4^2=16$, when $n=2$, an even number. Therefore $P(2)$ is also true.
#### Step 2: Inductive Step
*Show that for every integer $k\ge1$, if $P(i)$ is true for each integer from 1 through $k$, then $P(k+1)$ is also true.*
****
**Inductive Hypothesis:** For any integer $k\ge2$, each integer $i$ such that $0<i\le k$, the units digit of $4^i$ is 4 if $i$ is odd and 6 if $i$ is even.
$P(k+1)$: We must show that $4^{k+1}$ has a units digit of 4 when $k+1$ is odd and 6 when $k+1$ is even.
****
##### Case 1: $k+1$ is odd
Let $k$ be some even integer so that $k+1$ is odd.
$$
\begin{align}
4^{k+1}=& 4^k\cdot4 && \text{Exponent Properties} \\
\star_1=&(10q+6)\cdot4 && \text{Inductive Hypothesis} \\
=&40q+24 && \text{Distribute} \\
=&40q+20+4 && \text{Split Terms} \\
=&10(4q+2)+4 && \text{Distributive} \\
=&10r+4 && \text{For some integer }r
\end{align}
$$
$$\star_1\text{: Let q be some non-negative integer.}$$
Because the expression can be written as $10r+4$, then the units digit must be 4 for some odd integer $k+1$.
##### Case 2: $k+1$ is even
Let $k$ be some odd integer so that $k+1$ is even.
$$
\begin{align}
4^{k+1}=& 4^k\cdot4 && \text{Exponent Rules} \\
\star_2=&(10q+4)\cdot4 && \text{Inductive Hypothesis} \\
=& 40l+16 && \text{Distribute} \\
=& 40l+10+6 && \text{Split Terms} \\
=& 10(4l+1)+6 && \text{Distributive} \\
=& 10r+6 && \text{For some integer }r
\end{align}
$$
$$\star_2\text{: Let l be some non-negative integer.}$$
Because the expression can be written as $10r+6$, then the units must be 6 for some even integer $k+1$.
****
Because the two possible cases lead to correct conclusions with respect to the assumption, we can say that the units digit of $4^n$ for some positive integer $n$ is 4 when $n$ is odd and 6 when $n$ is even.
```

# 5.6

## 4

Find the first four terms of the sequence

$d_k=k(d_{k-1})^2$, for every integer $k\ge1$
$d_0=3$
```ad-answer
$$
\begin{align}
k=1: d_1 =& 1(d_0)^2, d_0=3 \to d_1=9 && (2) \\
k=2: d_2 =& 2(d_1)^2, d_1=9\to d_2=162 && (3) \\
k=3: d_3 =& 3(d_2)^2, d_2=162\to d_3=78732 && (4)
\end{align}
$$
$d_0=3$ is given, so the first 4 terms of the recursively defined sequence are:
$$
\boxed{3,9,162,78732}
$$
```

## 12

Let $s_0,s_1,s_2,...$ be defined by the formula $s_n= \frac{(-1)^n}{n!}$ for every integer $n\ge0$. Show that this sequence satisfies the following recurrence relation for every integer $k\ge1$:
$$s_k= \frac{-s_{k-1}}{k}$$
```ad-answer
Let $k$ be an integer with $k\ge 1$. Then $k-1\ge0$ is also true. Because $s_n= \frac{(-1)^n}{n!}$ is true for all integers $n\ge 0$, we can say that $s_n= \frac{(-1)^n}{n!}$ is true for both $n=k$ and $n=k-1$. This observation yields the following expressions for $k\ge 1$:
$$
s_k= \frac{(-1)^k}{k!}\quad\text{and}\quad s_{k-1}= \frac{(-1)^{k-1}}{(k-1)!}
$$
##### I will prove the recurrence relation with the brute force method.
$$
\begin{align}
s_k=& \frac{(-1)^k}{k!} \\
=& \frac{(-1)^k}{k(k-1)!} && \text{Factorial Rules} \\
=& \frac{(-1)^1(-1)^{k-1}}{k(k-1)!} && \text{Exponent Rules} \\
=& \frac{-(-1)^{k-1}}{k(k-1)!} && \text{Simplify} \\
=& \frac{-(-1)^{k-1}}{(k-1)!}\cdot\frac{1}{k} && \text{Factor out} \\
=& -s_{k-1}\cdot\frac{1}{k} && \text{Substitute }s_{k-1} \\
s_k=& \frac{-s_{k-1}}{k} && \text{Combine Terms}
\end{align}
$$
The conclusion derived above is equivalent to that proposed in the question, so the recurrence relation has been proved to be true.
```

## 38

*Compound Interest*: Suppose a certain amount of money is deposited in an account paying 3% annual interest compounded monthly. For each positive integer $n$, let $S_n=$ the amount on deposit at the end of the $n$th month, and let $S_0$ be the initial amount deposited.

### a

Find a recurrence relation for $S_0,S_1,S_2,...$, assuming no additional deposits or withdrawals during the year. Justify your answer.
```ad-answer
The interest is compounded monthly, so the monthly interest rate is:
$$\frac{3\%}{12}=0.25\%=0.0025$$
This means the amount deposited at the first month is $S_1=S_0+0.0025\cdot S_0$, where $S_0$ is the previous month.
This relationship is true for all months, so we can define the recurrence relation:
$$
\boxed{S_k=S_{k-1}+0.0025S_{k-1}=1.0025S_{k-1}}
$$
```

### b

If $S_0=$ $10,000, find the amount of money on deposit at the end of one year.
```ad-answer
The end of the year is the $12^{\text{th}}$month, so we can write the relation above as:
$$
\begin{align}
S_{12}=&1.0025S_{11} \\
=& (1.0025)^{12}\cdot S_0 \\
=& (1.0025)^{12}\cdot 10000 \\
=& \boxed{\$10,304.16}
\end{align}
$$
```

### c

Find the APY for the account.
```ad-answer
The Annual percentage yield (APY) is the percentage increase in the value of the account over a one-year period.
$$
\frac{10,304.16-10,000}{10,000}=0.030416=\boxed{3.0416\%}
$$
```

#### Thank you to Trevor Nichols for copying textbook questions into a markdown format 