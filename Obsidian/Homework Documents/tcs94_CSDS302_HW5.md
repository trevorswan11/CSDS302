# **CSDS302 HW5 - Trevor Swan (*tcs94*)**
# 4.5

## 14

If today is Tuesday, what day of the week will it be 1,000 days from today?
```ad-answer
$\text{Day}_N =(\text{Day}_T +N)\mod 7$
Let $\text{Day}_T = 2$, as today is tuesday.
Let $N = 1000$ as we are interested in 1000 days from today
$\therefore \text{Day}_{1000} = 1002 \mod 7$
$\frac{1002}{7} = 142 + \frac{1}{7} \therefore 1002\mod 7 = 1$
****
We can conclude that 1000 days from today, assuming today is Tuesday, is a Monday becuase $10002 \mod 7 = 1$ and 1 is representative of Monday.
```

## 21

Suppose $b$ is any integer. If $b\mod12=5$, what is $8b \mod 12$? In other words, if division of $b$ by $12$ gives a remainder of $5$, what is the remainder when $8b$ is divided by $12$? Your solution should show that you obtain the same answer no matter what integer you start with.
```ad-answer
If $b\mod 12 = 5$, then $b = 12n + 5$ for some integer $n$
$\therefore 8b = 8(12n+5) = 96n+40$
We can factor this solution to yield $8b = 96n + 36 + 4 = 12(8n+3) + 4$
Because $n$ is an integer, $8n+3$ is also an integer and we can say:
$8b = 12m + 4$ for some integer $m$
****
$\therefore$ We can rewrite the above statement as $8b\mod 12 = 4$, concluding that if $b\mod 12 =5$, then $8b\mod 12 = 4$. In other words the division of 8b by 12 in this case yields a remainer of 4 for any integer b that satisfies $b\mod 12=5$.
```

## 24

Prove that for all integers $m$ and $n$, if $m \mod 5=2$ and $n \mod 5=1$ then $mn \mod 5=2$.
```ad-answer
We can say that $m\mod 5 = 2$ is the same as $m = 5r_1+2$ for some integer $r_1$.
We can also say that $n\mod 5=1$ is the same as $n=5r_2+1$ for some integer $r_2$
$\therefore m\times n = (5r_1 + 2)(5r_2 + 1)$
FOIL the Expression:
$m\times n = 25r_1r_2 + 5r_1 + 5r_2 + 2$
Because $r_1$ and $r_2$ are both integers, we can define a new integer $r_3$
$\therefore m\times n = 5(5r_1r_2 + r_1 + r_2) + 2 = 5r_3 + 2$.
****
By the deifnition of the modulus operation, we can then conclude that $m\times n = 5r_3 + 2,r_3\in\mathbb{Z} \implies \boxed{mn\mod 5 = 2}.$
```

## 38

Prove the statement

For every integer $m$, $m^2=5k$, or $m^2=5k+1$, or $m^2=5k+4$ for some integer $k$.
```ad-answer
Let $m$ be an integer.
We must prove that $m = 5r + n$ for some $n<5$. I will do this through division into cases.
#### Case 1: $n=0$
$$
\begin{align}
m =& 5r && \text{Given} \\
m^2 =& (5r)^2 && \text{Substitution} \\
m^2 =& 25r^2 && \text{Expand} \\
m^2 =& 5(5r^2) && \text{Simplify} \\
\end{align}
$$
$5r^2$ is an integer for all $r\in\mathbb{Z}$
Let $k$ be some integer such that $k = 5r^2$ 
$\therefore \boxed{m^2 = 5k}$
#### Case 2: $n=1$
$$
\begin{align}
m=& 5r+1 && \text{Given} \\
m^2 =& (5r+1)^2 && \text{Substitute} \\
m^2 =& 25r^2 + 10r + 1 && \text{Expand} \\
m^2 =& 5(5r^2 +2r) +1 && \text{Simplify} \\
\end{align}
$$
$5r^2 +2r$ is an integer for all $r\in\mathbb{Z}$
Let $k$ be some integer such that $k = 5r^2 + 2r$
$\therefore \boxed{m^2 = 5k+1}$
#### Case 3: $n = 2$
$$
\begin{align}
m =& 5r+2 && \text{Given} \\
m^2 =& (5r+2)^2 && \text{Substitute} \\
m^2 =& 25r^2 + 20r + 4 && \text{Expand} \\
m^2 =& 5(5r^2 +4r) + 4 && \text{Simplify} \\
\end{align}
$$
$5r^2 +4r$ is an integer for all $r\in\mathbb{Z}$
Let $k$ be some integer such that $k = 5r^2 + 4r$
$\therefore \boxed{m^2 = 5k+4}$
#### Case 4: $n =3$
$$
\begin{align}
m =& 5r+3 && \text{Given} \\
m^2 =& (5r+3)^2 && \text{Substitute} \\
m^2 =& 25r^2 + 30r + 9 && \text{Expand} \\
m^2 =& 25r^2 + 30r + 5 + 4 && \text{Split Terms} \\
m^2 =& 5(5r^2 +6r+1) + 4 && \text{Simplify} \\
\end{align}
$$
$5r^2 +6r+1$ is an integer for all $r\in\mathbb{Z}$
Let $k$ be some integer such that $k = 5r^2 + 6r+1$
$\therefore \boxed{m^2 = 5k+4}$
#### Case 5: $n =4$
$$
\begin{align}
m =& 5r+4 && \text{Given} \\
m^2 =& (5r+4)^2 && \text{Substitute} \\
m^2 =& 25r^2 + 40r + 16 && \text{Expand} \\
m^2 =& 25r^2 + 40r + 15 + 1 && \text{Split Terms} \\
m^2 =& 5(5r^2 +8r+3) + 1 && \text{Simplify} \\
\end{align}
$$
$5r^2 +8r+3$ is an integer for all $r\in\mathbb{Z}$
Let $k$ be some integer such that $k = 5r^2 + 8r+3$
$\therefore \boxed{m^2 = 5k+1}$
#### Conclusion
For all choices of $n$ that satisfy $m =5r + n$, the only possible conclusions of $m^2$ are the following:
$$
\begin{align}
m^2 =& 5k \\
m^2 =& 5k+1 \\
m^2 =& 5k+4 \\
\end{align}
$$
This proves the requested statement for division of cases, as $n \in\set{0,1,2,3,4}$ must be true. $\square$
```

# 4.6

## 7

If $k$ is an integer, what is $\left\lfloor k+ \frac{1}{2}\right\rfloor$? Why?
```ad-answer
The floor function is defined as being the largest integer greater than or equal to the inputed value. Because k is an integer, than $k+\frac{1}{2}$ will be exactly $\frac{1}{2}$ greater than the input k. This means that the following must be true:
$$
\left\lfloor{k+\frac{1}{2}}\right\rfloor = k
$$
In conclusion, the expression in the question must be equal to k for all $k\in\mathbb{Z}$.
```

## 19-20

Some of the statements in 19-20 are true and some are
false. Prove each true statement and find a counterexample for each false statement, but do not use theorem 4.6.1 in your proofs.

### 19

For every real number $x$, $\left\lceil x-1\right\rceil=\lceil x\rceil-1$
```ad-answer
I will prove this using Division into cases with a generic particular
For the following, let $n$ be some arbitrary number.
#### Case 1: $n \in\mathbb{Z}$
**LHS:** $\lceil{n-1}\rceil = n-1$ by the definition of the celing function.
**RHS:** $\lceil{n}\rceil = n$ by the definition of the celing function so we can say that $\lceil{n}\rceil - 1 = n - 1$.
**In conculstion:** $\boxed{n - l = n - 1}$ $\qquad$*True* $\checkmark$
#### Case 2: n $\not\in\mathbb{Z}$
*In the following, I am using the java typecast notation to truncate n when indicated by the (int) operator*
**LHS:** $\lceil{n-1}\rceil = (int)n$ because $n-1$ will be slighly less than n and the ceiling function returns the least greatest integer.
**RHS:** $\lceil{n}\rceil = (int)n+1$ becuase the ceiling function will return the least greatest integer above the input. This side of the expression evaluates to $n + 1 - 1 = n$
**In conclusion:** $\boxed{n = n}$ $\qquad$*True* $\checkmark$
#### Therefore...
Because the two possible choices of n (being an integer and not) lead to true statements, the given equation must be true. $\square$
```

### 20

For all real numbers $x$ and $y$, $\lceil xy\rceil=\lceil x\rceil\cdot\lceil y\rceil$
```ad-answer
This is a false statement, and I will disprove it with a counterexample.
$$
\begin{align}
\text{Let}\quad x =& y = 2.5 \\ 
\text{Evaluate LHS}\quad \lceil{xy}\rceil =& \lceil{6.25}\rceil = 7 \\
\text{Evaluate RHS}\quad \lceil{x}\rceil =& \lceil{y}\rceil = \lceil{2.5}\rceil = 3 \\
\therefore& \lceil{x}\rceil \cdot \lceil{y}\rceil = 9 \\
6.25 \neq& 9
\end{align}
$$
Because this example is incorrect, the statement cannot be true!
```

# 4.7

## 4

Use proof by contradiction to show that for every integer $m$, $7m+4$ is not divisible by $7$.
```ad-answer
Assume that an integer m exists such that $7m+4$ *is* divisible by 7.
**Divisbility Definition**
States that if $d\mid n$ then n is divisible by d if and only if an integer $k$ exists such that n = dk.
#### Pf/
Using this definition we can say the following:
$$
\begin{align}
7m +4 =& 7k && \text{For some integer k} \\
4 =& 7k-7m && \text{Subtract variable m term} \\
4 =& 7(k-m) && \text{Factor out the 7} \\
4 =& 7n && \text{For some integer n} \\
\end{align}
$$
$\therefore 7\mid 4$ must be true by the definition of divisibility.
For the statement $d\mid n$ to be true, $d\le n$ must also be true.
But $7 > 4$.
Thus we have derived a contradiction showing that for any integer $m, 7m+4$ is not divisible by 7. $\square$
```

## 6

Carefully formulate the negations of the statement. Then prove it by contradiction.

There is no greatest negative real number.
```ad-answer
The negation of the statement is:
"There is a greatest negative real number."
I will disprove this statement using contradiction.
#### Pf/
Assume there is some greatest negative real N.
We can define a new number N' where $N' = N -1$
Comparing the two numbers yields the following:
$$
N < N'
$$
This is true as N' is one less than N, making it more negative.
But we assumed N was the greatest negative real number.
This leads to the contradiction found above, thus proving that there is no greatest negative real number. $\square$
```

## 17

Prove the statement by contradiction

For all prime numbers $a,b,c$, $a^2+b^2\ne c^2$
```ad-answer
#### Pf/
Assume that for some primes, $a,b,\text{ and }c$, $a^2 +b^2 = c^2$ is true.
We can then say the following:
$$
\begin{align}
a^2 + b^2 =& c^2 && \text{Given} \\
a^2 =& c^2 - b^2 && \text{Subtract }c^2\text{ from each side} \\
a^2 =& (c-b)(c+b) && \text{Difference of squares} \\
\end{align}
$$
We can then say that $b\ge c -1 \equiv c-b \ge 1$
This introduced two possible cases.
#### Case 1: $c-b = 1$
Let $c=3$ and $b = 2$ to satisfy the constraints
We can say:
$$
\begin{align}
a^2 =& (3-2)(3+2) && \text{Substitute} \\
a^2 =& 5 && \text{Evaluate} \\
a =& \sqrt{5} && \text{Simplify}
\end{align}
$$
For $a$ to be prime, it must be a positive intgeger. Here, however, $a = \sqrt{5}$.
5 is not a perfect square, so $a$ cannot be an integer. Leading to a contradiction.
Because this case leads to a contradiction, the other case doesnt need to be considered as one contradiction leads to the full disproval of a statement.
#### In conclusion:
Since, when the criteria is $c - b = 1$, to satisfy the equation above is met, the result of $a=\sqrt{5}$ is reached. In this case, a is not an integer so a is not prime. This lets us say that for all primes $a, b,\text{ and }c, a^2 + b^2 \neq c^2$. $\square$
```

# 4.8

## 14

Determine whether the statement is true or false. Prove it if it is true and disprove it if it is false.

The sum of any two positive irrational numbers is irrational.
```ad-answer
This satement is false.
Suppose we have an irrational number $r$ and a rational number $n$.
We can define two new numbers $a$ and $b$ where the following is true:
$$
\begin{align}
a =& r \\
b =& n - r \\
\end{align}
$$
Both of these terms are irrational because the difference between a rational and irrational number is irrational.
Define some number $m$.
We can say that $m = r + (n -r)$, the sum of $a$ and $b$.
This sum evaluates to $m = n$.
Since $n$ is an integer, m is also an integer.
But the problem requested an irrational sum.
Therefore the given statement is false becuase $a + b$, as defined above, results in a rational number $m$. $\square$
```

## 23

Prove that for any integer $a$, $9 \nmid(a^2-3)$.
```ad-answer
I will prove the following using contradiction.
#### Pf/
Assume that a positive integer $a$ exists where $9\mid (a^2 - 3)$.
By the definition of divisibility, an integer $k$ exists where $(a^2 - 3) = 9k$ is a true statement.
We can then draw the following conclusions:
$$
\begin{align}
(a^2 - 3) =& 9k && \text{Given} \\
a^2 =& 9k+3 && \text{Add 3 from each side} \\
a^2 =& 3(3k+1) && \text{Factor out the 3} \\
a^2 =& 3n && \text{Define an integer n where }n=3k+1 \\
\end{align}
$$
We can see that $a^2$ is divisible by 3, so we can rewrite a as $a=3m$ for some integer $m$.
Therefore we can say the following:
$$
\begin{align}
a =& 3m && \text{Given} \\
a^2 =& 9m^2 \text{Substitute} \\
a^2 =& 3(3m^2) \text{Factor out 3}
\end{align}
$$
We can then set thesse two equal to eachother:
$$
\begin{align} 
3n =& 3(3m^2) && \text{Given} \\
n =& 3m^2 && \text{Divide by 3} 
\end{align}
$$
This derives a contradiction because n must be a multiple of 3 for the above statement to be true. This is never stated above, so there is nothing that can guarantee the truth of the above conclusion.
Therefore we can say that for *any* integer $a, 9\nmid (a^2 - 3)$
```

# 4.10

## 15-16

Use the Euclidean algorithm to hand-calculate the greatest common divisors of each of the pairs of integers in 15–16.

### 15

$832$ and $10933$
```ad-answer
#### Step 1: Divide 10933 by 832
$$ 
\require{enclose} 
\begin{array}{rll} 13 \\[-3pt] 
832 \enclose{longdiv}{10933}\kern-.2ex \\[-3pt] 
\underline{832\phantom{0}} \\[-3pt] 
2613\phantom{} \\[-3pt] 
\underline{\phantom{}2496\phantom{}} \\[-3pt] 
\phantom{0}117 && \leftarrow\text{Remainder}\\[-3pt] 
%\underline{\phantom{0}20} \\[-3pt]
%\phantom{00}0 
\end{array} 
$$
$\therefore\gcd(10933,832) = \gcd(832, 117)$
#### Step 2: Divide 832 by 117
$$ 
\require{enclose} 
\begin{array}{rll} 7 \\[-3pt] 
117 \enclose{longdiv}{832}\kern-.2ex \\[-3pt] 
\underline{819\phantom{}} \\[-3pt] 
13\phantom{} && \leftarrow\text{Remainder} \\[-3pt] 
%\underline{\phantom{}2496\phantom{}} \\[-3pt] 
%\phantom{0}117 \\[-3pt] 
%\underline{\phantom{0}20} \\[-3pt]
%\phantom{00}0 
\end{array} 
$$
$\therefore\gcd(832,117) = \gcd(117,13)$
#### Step 3: Divide 117 by 13
$$ 
\require{enclose} 
\begin{array}{rll} 9 \\[-3pt] 
13 \enclose{longdiv}{117}\kern-.2ex \\[-3pt] 
\underline{117\phantom{}} \\[-3pt] 
0\phantom{} && \leftarrow\text{Remainder} \\[-3pt] 
%\underline{\phantom{}2496\phantom{}} \\[-3pt] 
%\phantom{0}117 \\[-3pt] 
%\underline{\phantom{0}20} \\[-3pt]
%\phantom{00}0 
\end{array} 
$$
$\therefore\gcd(117,13)=\gcd(13,0)$
#### Conclusion
$\gcd(13,0)=13$ by lemma $4.10.1$. The greatest common divisor of 10933 and 832 is $\boxed{13}$.
```

### 16

$4131$ and $2431$
```ad-answer
#### Step 1: Divide 4131 by 2431
$$ 
\require{enclose} 
\begin{array}{rll} 1 \\[-3pt] 
2431 \enclose{longdiv}{4131}\kern-.2ex \\[-3pt] 
\underline{2431\phantom{}} \\[-3pt] 
1700\phantom{} && \leftarrow\text{Remainder} \\[-3pt] 
%\underline{\phantom{}2496\phantom{}} \\[-3pt] 
%\phantom{0}117 \\[-3pt] 
%\underline{\phantom{0}20} \\[-3pt]
%\phantom{00}0 
\end{array} 
$$
$\therefore\gcd(4131,2431)=\gcd(2431,1700)$
#### Step 2: Divide 2431 by 1700
$$ 
\require{enclose} 
\begin{array}{rll} 1 \\[-3pt] 
1700 \enclose{longdiv}{2431}\kern-.2ex \\[-3pt] 
\underline{1700\phantom{}} \\[-3pt] 
731\phantom{} && \leftarrow\text{Remainder} \\[-3pt] 
%\underline{\phantom{}2496\phantom{}} \\[-3pt] 
%\phantom{0}117 \\[-3pt] 
%\underline{\phantom{0}20} \\[-3pt]
%\phantom{00}0 
\end{array} 
$$
$\therefore\gcd(2431,1700)=\gcd(1700,731)$
#### Step 3: Divide 1700 by 731
$$ 
\require{enclose} 
\begin{array}{rll} 2 \\[-3pt] 
731 \enclose{longdiv}{1700}\kern-.2ex \\[-3pt] 
\underline{1462\phantom{}} \\[-3pt] 
238\phantom{} && \leftarrow\text{Remainder} \\[-3pt] 
%\underline{\phantom{}2496\phantom{}} \\[-3pt] 
%\phantom{0}117 \\[-3pt] 
%\underline{\phantom{0}20} \\[-3pt]
%\phantom{00}0 
\end{array} 
$$
$\therefore\gcd(1700,731)=\gcd(731,238)$
#### Step 4: Divide 731 by 238
$$ 
\require{enclose} 
\begin{array}{rll} 3 \\[-3pt] 
238 \enclose{longdiv}{731}\kern-.2ex \\[-3pt] 
\underline{714\phantom{}} \\[-3pt] 
17\phantom{} && \leftarrow\text{Remainder} \\[-3pt] 
%\underline{\phantom{}2496\phantom{}} \\[-3pt] 
%\phantom{0}117 \\[-3pt] 
%\underline{\phantom{0}20} \\[-3pt]
%\phantom{00}0 
\end{array} 
$$
$\therefore\gcd(731,238)=\gcd(238,17)$
#### Step 5: Divide 238 by 17
$$ 
\require{enclose} 
\begin{array}{rll} 14 \\[-3pt] 
17 \enclose{longdiv}{238}\kern-.2ex \\[-3pt] 
\underline{17\phantom{0}} \\[-3pt] 
68\phantom{}  \\[-3pt] 
\underline{\phantom{}68\phantom{}} \\[-3pt] 
\phantom{0}0 && \leftarrow\text{Remainder} \\[-3pt] 
%\underline{\phantom{0}20} \\[-3pt]
%\phantom{00}0 
\end{array} 
$$
$\therefore\gcd(238,17)=\gcd(17,0)$
#### Conclusion
$\gcd(17,0)=17$ by lemma 4.10.1. The greatest common divisor of 4131 and 2431 is $\boxed{17}$.
```

# 5.1

## 6

Write the first four terms of the sequence

$f_n=\left\lfloor \frac{n}{4}\right\rfloor\cdot 4$ for every integer $n\ge 1$
```ad-answer
#### Determine values for $n\in\set{1,2,3,4}$
$$
\begin{align}
n =&1: \left\lfloor{\frac{1}{4}}\right\rfloor\cdot4 = \lfloor{0.25}\rfloor \cdot4 = 0\cdot4 =0 \\
n =&2: \left\lfloor{\frac{2}{4}}\right\rfloor\cdot4 = \lfloor{0.50}\rfloor \cdot4 = 0\cdot4 =0 \\
n =&3: \left\lfloor{\frac{3}{4}}\right\rfloor\cdot4 = \lfloor{0.75}\rfloor \cdot4 = 0\cdot4 =0 \\
n =&: \left\lfloor{\frac{4}{4}}\right\rfloor\cdot4 = \lfloor{1}\rfloor \cdot4 = 1\cdot4 =4 \\
\end{align}
$$
Based on the calculated values above, the first 4 terms in the sequence $f_n=\left\lfloor \frac{n}{4}\right\rfloor\cdot 4$ for integers $n\ge1$ are $\boxed{0,0,0,4}$.
```

## 60

Rewrite as a single summation or product

$2\cdot\sum\limits_{k=1}^n(3k^2+4)+5\cdot\sum\limits_{k=1}^n(2k^2-1)$
```ad-answer
$$
\begin{align}
2\cdot\sum\limits_{k=1}^n(3k^2+4)+5\cdot\sum\limits_{k=1}^n(2k^2-1) =& ? \\
\textit{(Multiply Scalars)}=& \sum\limits_{k=1}^n2\cdot(3k^2+4) + \sum\limits_{k=1}^n5\cdot(2k^2-1) \\
\textit{(Distributive)}=&\sum\limits_{k=1}^n((6k^2+8) + (10k^2-5)) \\
\textit{(Combine Terms)}=&\sum\limits_{k=1}^n(16k^2+3) \\
\therefore2\cdot\sum\limits_{k=1}^n(3k^2+4)+5\cdot\sum\limits_{k=1}^n(2k^2-1) =& \boxed{\sum\limits_{k=1}^n(16k^2+3)}
\end{align}
$$
*Note that in the 'distributive' step, I was able to combine the summations because of the identical bounds*
```

#### Thank you to Trevor Nichols for copying textbook questions into a markdown format 