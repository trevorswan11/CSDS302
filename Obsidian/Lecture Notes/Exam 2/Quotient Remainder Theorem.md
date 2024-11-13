````ad-theory
title: Theorem
$$
\begin{align}
\forall n,d\in&\mathbb{Z} \\
n =& d\cdot q + r && 0\le r\le d \\
\end{align}
$$
*R is the remainder*
If $r = 0$
$n = d\cdot q, d|n$
#### Modulus/Remainder:
$$
n\text{ mod }d = r
$$
```ad-example
10 mod 3 = 1
$10 = 3\times 3 + 1$
```
#### Or you can use 'div'
$$
n\text{ div }d = q
$$
```ad-example
10 div 3 = 3
```
````
#### Examples
```ad-example
title: Consider... 
Today is Monday, what day is 365 days from now
$365 = 7\times52+1$
```
```ad-example
title: Example 1: Consider $m\in\mathbb{Z}$
#### *If m mod 11 = 6, what is 4m mod 11?*
$m = 11q + 6$
$4m = 44q + 24 = 44q + 22 + 2 = 11(4q+2) + 2\therefore 4m\text{ mod }11 = 2$
```
#### Another Thm
````ad-theory
The Square of any odd integer has the form $8m+1,m\in\mathbb{Z}$
*This is equivalent to saying the square of any integer mod 8 = 1.*
```ad-example
$$
\begin{align}
7^2 = 49&&\text{ Then }\dots &&49\mod8 = 1
\end{align}
$$
```
#### Now we will prove...
$\forall n\in\mathbb{Z}, n$ can be written as one of the following forms
$$
\begin{align}
4q&&4q+1&&4q+2&&4q+3
\end{align}
$$
*Notice how there is no $4q+4$ as that is divisible by 4 and can be represented as $4q$*
****
**We can then say the following**
$$
2q\qquad2q+1
$$
Where 2q is even and 2q+1 is od
#### Case 1: n = 4q+1
$$
\begin{align}
(4q+1)^2 =& 16q^2 + 8q + 1 \\
=& 8(2q^2+q) + \boxed{1} \\
\end{align}
$$
Where we can call $2q^2 + q$ 'm'
#### Case 2: n = 4q+3
$$
\begin{align}
(4q+3)^2 =& 16q^2 + 24q + 9 \\
=& 8(2q^2 + 3q + 1) + \boxed{1} \\
\end{align}
$$
Where we can call $2q^2 + 3q + 1$ 'm'
#### Conclsion:
We can see that the square of any odd integer has the form $8m+1$
Furthermore, we can conlcude that $(\text{Any Odd Integer})^2\text{ mod }8 = \boxed{1}$
````
