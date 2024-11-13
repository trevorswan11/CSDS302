# **CSDS302 HW4 - Trevor Swan (*tcs94*)**
# 4.1

## 9-11

Prove the statements in 9–11.

### 9

There is a real number $x$ such that $x>1$ and $2^x>x^{10}$.
```ad-answer
Suppose there is a real number x that is greater than one. Let $x=1.05$, which satisfies the condition x > 1.
If x = 1.05, then...
$$
\begin{align}
2^x =& 2^{1.05} \approx 2.07 \\
x^{10} =& 1.05^{10} \approx 1.63
\end{align}
$$
From these calcualtions, it can be concluded that $2^{1.05}>1.05^{10}$ as $2.07>1.63$. 
$\therefore$ There is a real number $x$ such that $x>1$ and $2^x>x^{10}$.
```

### 11

There is an integer $n$ such that $2n^2-5n+2$ is prime.
```ad-answer
Suppose there is an integer n such that $2n^2-5n+2$. It is known that prime numbers are positive integers that are divisible only by 1 and themselves. Therefore, n must be an integer such that $2n^2-5n+2$ satisfies these conditions.
$$
\begin{align}
\text{Factor the polynomial:}&& &2n^2-5n+2 = (2n-1)(n-2) \\
\text{Find n values where factors = 1}&& &2n-1 = 1 \text{ or } n-2 = 1 \\
\text{Solve for n in each case:}&& &n = 1 \text{ or } n = 3 \\
\end{align}
$$
$$
\text{Evaluate the Polynomial at the evaluated n values above.} \\
$$
$$
\begin{align}
n=1 && &2n^2-5n+2|_{n=1} = 2(1)^2-5(1)+2 = -1 \\
n=3 && &2n^2-5n+2|_{n=3} = 2(3)^2 -5(3)+2 = 5 \\
\end{align}
$$
As mentioned above, prime numbers are only defined for positive integers, and 5 is prime.
$\therefore$ There is an integer $n$ such that $2n^2-5n+2$ is prime.
```

## 25

The statement is true. For each, (a) rewrite the statement with the quantification implicit as If \_\_\_\_, then \_\_\_\_, and (b) write the first sentence of a proof (the “starting point”) and the last sentence of a proof (the “conclusion to be shown”).
(Note that you do not need to understand the statements in order to be able to do these exercises.)

For all integers $m$ and $n$, if $mn=1$ then $m=n=1$
or $m=n=-1$.
```ad-answer
(a) If $m$ and $n$ and integers such that $mn = 1$, then $m=n=1$ or $m=n=-1$.

(b) **First Sentence of Proof:** Suppose m and n are integers such that $mn = 1$.
$\quad$ **Last Sentence of Proof:** $m=n=1\text{ or }m=n=-1$.
```

# 4.2

## 13

Prove that the statement is false

There exists an integer $n$ such that $6n^2+27$ is prime.
```ad-answer
Prime numbers must not be divisible by any number than itself and 1. 
Suppose an integer n is part of a function where $6n^2 +27$ gives an integer output. 
Through basic algebra...
$$
6n^2+27 = 3(2n^2+9)
$$
Becuase the factorization of this function reveals a scalar of 3, every output will be divisible by 3 since n is an integer.
$\therefore$ There is no integer n such that $6n^2+27$ is prime.
```

## 27

Determine whether the statement is true or false. Justify your answer with a proof or a counterexample, as appropriate. In each case use only the definitions of the terms and the assumptions listed on page 161, not any previously established properties.

The difference of any two odd integers is even.
```ad-answer
This statement is true, as proved below using the generalization from the generic particular.
Suppose we have 2 odd integers: $m = 2k+1$ and $n=2r+1$, where $r,k\in\mathbb{Z}$.
The differernce of these integers can be shown below:
$$
\begin{align}
m - n =& (2k+1)-(2r+1) \\
=& 2k-2r \\
=& 2(k-r) \\
\end{align}
$$
Even integers are defined as 2 times some number n. We can let w = (k-r), and substiture this value into the equaiton above, giving:
$$
m-n = 2w
$$
$\therefore$ The difference between two odd integers is even as their difference can be represented as 2w, the definition of an even integer.
```

# 4.3

## 2-7

The numbers in 2–7 are rational. Write each number as a ratio of two integers.

### 2

$4.6037$
```ad-answer
A ratio of two integers is easy to write here, all that needs to be done is to multiply 4.6037 by $\frac{10,000}{10,000}$.
This gives the answer of $\frac{46,037}{10,000}$.
```

### 7

$52.4\overline{6721}$
```ad-answer
Let $x=52.4\overline{6721}$. Then $10x = 524.\overline{6271}$ and $10000x = 5246721.\overline{6721}$. Thus
$$
\begin{align}
100000x - 10x =& 5246721.\overline{6721} - 524.\overline{6271} \\
=& 5246197 \\
\therefore 99990x =& 5246197 \\
x =& \frac{5246197}{99990}
\end{align}
$$
$\therefore$ The ratio of two integers for $52.4\overline{6721}$ is $\frac{5246197}{99990}$
```

# 4.4

## 5

Give a reason for your answer in each of 1–13. assume that all variables represent integers.

Is $6m(2m+10)$ divisible by $4$?
```ad-answer
n is divisible by d is and only if there exists some integer k such that n = dk.
$$
4|6m(2m+10)\text{ if }4k = n
$$
Assuming $m$ is an integer...
Using basic algebra, we can simplify the expression to the following:
$$
\begin{align}
6m(2m+10) =& 6m\cdot2(m+5) \\
=& 12m(m+5) \\
\therefore =& 4(3m(m+5)) \\
\end{align}
$$
Because 4 is a factor in the expression and we can guarantee that the expression is an integer, we can conclude that $6m(2m+10)$ is divisible by 4.
```

## 16

Prove the statement directly from the definition of divisibility.

For all integers $a,b,c$ if $a|b$ then $a|c$ then $a|(b-c)$.
```ad-answer
Consider $x,y,z\in\mathbb{Z}$
$$
\begin{align}
a|b\text{ then }b =& xa \\
a|c\text{ then }c =& ya \\
a|(b-c) &\text{ True? }\\
\end{align}
$$
$$
\text{Through Substitution we can conclude the following}
$$
$$
\begin{align}
ax - ay =& \text{?} \\
a(x-y) =& \text{?} \\
\end{align}
$$
Because $a,x,$ and $y$ are all integers, the expression $a(x-y)$ must yield an integer as well, showing that the statement $a|(b-c)$ is true.
```

## 21

For the statement, determine whether the statement is true or false. Prove the statement directly from the definitions if it is true, and give a counterexample if it is false.

The product of any two even integers is a multiple of $4$.
```ad-answer
Let two even intgers x and y be defined as $x = 2a$ and $y= 2b$.
The product of these two integers can be represented as:
$$
\begin{align}
x\times y =& 2a\times 2b \\
=& 4ab
\end{align}
$$
Through the definition of divisibility, we can see that:
$$
4|4ab \to 4ab = 4k \qquad\text{For some integer } k
$$
Because a and b are both integers, their product will be an integer proving that  $4|4ab$ is true.
```

## 35

Two athletes run a circular track at a steady pace so that the first completes one round in 8 minutes and the second in 10 minutes. If they both start from the same spot at 4 p.m., when will be the first time they return to the start together?
```ad-answer
Let the two runners be represented by $a = 8t$ and $b=10t$ where the first runner $a$ runs a track at a steady pace of 8min/lap and runner $b$ completes a lap every 10 minutes.
- Runner $a$'s lap time is the set $\set{10,20,30,40,50\dots}$
- Runner $b$'s lap time is the set $\set{8,16,24,32,40,48\dots}$
The first common multiple the runners share is at 40 minutes, so the runners will meet at 4:40pm.
****
This problem can also be solved by looking for the first non-zero common divisor.
Through the definition of division, we can say that:
$$
a=8t \to 8|a\qquad\text{ and }\qquad b=10t \to 10|b
$$
For the runners to meet, the following must be true:
$$
8|m\qquad\text{ and }\qquad10|m
$$
This is fancier way of saying that m must be divisible by both 8 and 10.
We can simplify this by the expressions:
$$
4|m\qquad\text{ and }\qquad 5|m
$$
Logically, the expression is: $4|m\land 5|m$
For this to be true, $m$ must be equal to 40 to represent the first time, or first division, that causes the runners, or expressions, to be equal. This leaves us with th esame result as method one of 4:40pm.
```

#### Thank you to Trevor Nichols for copying textbook questions into a markdown format 