# **CSDS302 HW2 - Trevor Swan (*tcs94*)**
*Note about the 'not' operator: $\lnot$ is used instead of $\lnot$ for this entire document*
# 2.1
****
## 2

Represent the common form of each argument using letters to stand for component sentences, and fill in the blanks so that the argument in part (b) has the same logical form as the argument in part (a).

### a

If all computer programs contain errors, then this program contains an error. This program does not contain an error. Therefore, it is not the case that all computer programs contain errors.
 >[!answer]
 >Let $p=$ "all computer programs contain errors" and $q=$ "this program contains errors".
 >If $p$, then $q$. $\lnot q.\ \therefore \lnot q$
 
### b

If \_\_\_\_ then \_\_\_\_. 2 is not odd. Therefore, it is not the case that all prime numbers are odd.
 >[!answer]
 >If all prime numbers are odd, then 2 is odd. 2 is not odd. Therefore, it is not the case that all prime numbers are odd.
 >Let $p=$ "all prime numbers are odd" and $q=$ "2 is odd".
 >If $p$, then $q$. $\lnot q.\ \therefore \lnot q$


## 5

Indicate which of the following sentences are statements.

### b

She is a mathematics major.
 >[!answer]
 >This sentence is not specific enough to be classified as either true or false. "She" is an arbitrary and holds no real value when determining if this is a statement or not. This sentence **is not a statement.**
### c

$128=2^6$
 >[!answer]
 >$2^6 = 64$ would be a *true* statement, but even though the expression given is false, it is known to be false and therefore **is a statement.**


## 8

Write the statements in symbolic form using the symbols $\lnot,\land,\lor$ and the indicated letters to represent component statements.

Let $h=$“John is healthy,” $w=$“John is wealthy,” and $s$=“John is wise.”

### b

John is not wealthy but he is healthy and wise.
 >[!answer]
 >$\lnot w\land(h\land s)$
### e

John is wealthy, but he is not both healthy and wise.
 >[!answer]
 >$w\land \lnot(h\land s)$
## 10

Let $p$ be the statement “DATAENDFLAG is off,” $q$ the statement “ERROR equals 0,” and $r$ the statement “SUM is less than 1,000.” Express the following sentences in symbolic notation.

### b

DATAENDFLAG is off but ERROR is not equal to 0.
 >[!answer]
 >$p\land \lnot q$
### e

Either DATAENDFLAG is on or it is the case that both ERROR equals 0 and SUM is less than 1,000.
 >[!answer]
 >$\lnot p\lor(q\land r)$
## 15

Write truth tables for the statement $p\land(\lnot q\lor r)$
 >[!answer]
 >
| p | q | r | $\lnot q$ | $\lnot q \lor r$ | $p \land(\lnot q \lor r)$ |
| ---- | ---- | ---- | ---- | ---- | ---- |
| T | T | T | F | T | T |
| T | F | T | T | T | T |
| T | T | F | F | F | F |
| T | F | F | T | T | T |
| F | T | T | F | T | F |
| F | F | T | T | T | F |
| F | T | F | F | F | F |
| F | F | F | T | T | F |
## 19-24

Determine whether the statements are logically equivalent. Construct a truth table and include a sentence justifying your answer. Your sentence should show that you understand the meaning of logical equivalence.

### 19

$p\land \mathbf t$ and $p$
 >[!answer]
 >
| p | t | $p\land t$ |
| ---- | ---- | ---- |
| T | T | T |
| F | T | F |
>$p\land t \equiv p$ as the left hand side is only true when p is true, because 'and' requires both sides of the statement to be true. By definition, $t$ is always true, so p is logically equivalent to the expression $p \land t$. This is also proven by the identity law.
### 20

$p\land\mathbf c$ and $p\lor\mathbf c$
 >[!answer]
| p | c | $p\land c$ | $p\lor c$ |
| ---- | ---- | ---- | ---- |
| T | F | F | T |
| F | F | F | F |
Because p can be true, the or statement can also be true. Since, by definition, $c$ is always false, the two statements cannot be equivalent. $p\land c\not\equiv p\lor c$.
### 22

$p\land(q\lor r)$ and $(p\land q)\lor(p\land r)$
 >[!answer]
 >
| p | q | r | $q\lor r$ | $p\land(q\lor r)$ | $p\land q$ | $p\land r$ | $(p\land q)\lor(p\land r)$ |
| ---- | ---- | ---- | ---- | ---- | ---- | ---- | ---- |
| T | T | T | T | T | T | T | T |
| T | F | T | T | T | F | T | T |
| T | T | F | T | T | T | F | T |
| T | F | F | F | F | F | F | F |
| F | T | T | T | F | F | F | F |
| F | F | T | T | F | F | F | F |
| F | T | F | T | F | F | F | F |
| F | F | F | F | F | F | F | F |
Even without the use of this table, the distributive law states that the following is always true:
$p\land(q\lor r)\equiv(p\land q)\lor(p\land r)$.

### 24

$(p\lor q)\lor(p\land r)$ and $(p\lor q)\land r$
 >[!answer]
 >
| p | q | r | $p\lor q$ | $p\land r$ | $(p\lor q)\lor(p\land r)$ | $(p\lor q)\land r$ |
| ---- | ---- | ---- | ---- | ---- | ---- | ---- |
| T | T | T | T | T | T | T |
| T | F | T | T | T | T | T |
| T | T | F | T | F | T | F |
| T | F | F | T | F | T | F |
| F | T | T | T | F | T | T |
| F | F | T | F | F | F | F |
| F | T | F | T | F | T | F |
| F | F | F | F | F | F | F |
The last two columns are not equivalent, and since they represent the given statements, we can conclude that they are not equivalent. By the distributive law, $(p\lor q)\land r\equiv(p\land q)\lor(p\land r)$, a conclusion made after applying the associative law where $(p\lor q)\land r\equiv p\lor(q\land r)$. These two laws make it more than clear that $(p\lor q)\lor(p\land r)\not\equiv(p\lor q)\land r$.

## 29

Use De Morgan’s laws to write negations for the statement
"This computer program has a logical error in the first ten lines or it is being run with an incomplete data set."
 >[!answer]
 >Let $p=$ "This computer program has a logical error in the first ten lines" and $q=$ "This computer is being run with an incomplete data set". The given statement is $p\lor q$. By De Morgan's law, the negation of this statement is $\lnot(p\lor q)\equiv\lnot p\land\lnot q$. Therefore, the negation of this statement is as follows: **This computer program does not have a logical error in the first ten lines and it is being run with a complete data set**.
 

## 35

Assume x is a particular real number and use De Morgan’s laws to write negations for the statement
$x\le-1$ or $x>1$
 >[!answer]
 >Let $p=\ 'x\le -1'$ and $q=\ 'x>1'$. The given statement is $p \lor q$. To negate this statement, we can use De Morgan's Law to negate the individual statements and change all *or's* into *ands*' and *and's* into *or's* in the context of the problem. In words, the negation of the given statement is "x is greater than -1 and x is less than or equal to 1". Symbolically, this is represnted as $\lnot p\land \lnot q$ or $(x>-1)\land(x\le1)$.
 

## 43

Use truth tables to establish if the statement form is a tautology and if it is a contradiction.

$(\lnot p\lor q)\lor (p\land\lnot q)$
 >[!answer]
| p | q | $\lnot p$ | $\lnot q$ | $\lnot p\lor q$ | $p\land\lnot q$ | $(\lnot p\lor q)\lor(p\land\lnot q)$) |
| ---- | ---- | ---- | ---- | ---- | ---- | ---- |
| T | T | F | F | T | F | T |
| T | F | F | T | F | T | T |
| F | T | T | F | T | F | T |
| F | F | T | T | T | F | T |
As observed by the above truth table, all of the rows lead to a true conclusion, so the given statement form is a tautology.

## 49

A logical equivalence is derived from Theorem 2.1.1. Supply a reason for each step.

$(p\lor\lnot q)\land(\lnot p\lor\lnot q)$
$\qquad \equiv(\lnot q\lor p)\land(\lnot q\lor\lnot p)\qquad(by\ a)$
$\qquad \equiv\lnot q\lor(p\land\lnot p)\qquad(by\ b)$
$\qquad \equiv\lnot q\lor\mathbf c\qquad(by\ c)$
$\qquad \equiv\lnot q\qquad(by\ d)$
Therefore, $(p\lor\lnot q)\land(\lnot p\lor\lnot q)\equiv \lnot q$
 >[!answer]
 >**(a)** is by the commutative law 
 >$p\land q\equiv q\land p$<br>
 >**(b)** is by the distributive law 
 >$p\land(q\lor r)\equiv(p\land q)\lor (p\land r)$<br>
 >**(c)** is by the negation law 
 >$p\land c \equiv p$<br>
 >**(d)** is by the identity law
 >$p\lor c \equiv p$


## 51

Use Theorem 2.1.1 to verify the logical equivalence. Supply a reason for each step.
	LHS = Left Hand Side
$p\land(\lnot q\lor p)\equiv p$
```ad-answer
$$
\begin{align}
LHS &\equiv p \land(\lnot q\lor p) && Given\\
&\equiv p\land(p\lor\lnot q) && (a) \\
& \equiv p && (b)
\end{align}
$$
**(a)** is by the commutative law
$p\land q\equiv q\land p$ <br>
**(b)** is by the absorption law
$p\land(p\lor q)\equiv p$
```
 

# 2.2
****
## 2

Rewrite the statement in if-then form

I am on time for work if I catch the 8:05 bus
 >[!answer]
 >If I catch the 8:05 bus, then I am on time for work.
 

## 8

Construct truth tables for the statement form

$\lnot p\lor q\to r$
 >[!answer]
| p | q | r | $\lnot p$ | $\lnot p\lor q$ | $\lnot p \lor q\to r$ |
| ---- | ---- | ---- | ---- | ---- | ---- |
| T | T | T | F | T | T |
| T | F | T | F | F | T |
| T | T | F | F | T | F |
| T | F | F | F | F | T |
| F | T | T | T | T | T |
| F | F | T | T | T | T |
| F | T | F | T | T | F |
| F | F | F | T | T | F |
A good trick to writing truth tables like this is that the statement for $p\to q$ is only false when p is true and q is false. It is true in *all* other situations.
 

## 14

### b

$p\to q\lor r\equiv p\land \lnot q\to r\equiv p\land\lnot r\to q$

Use the logical equivalences above to rewrite the following sentence in two different ways. (Assume that n represents a fixed integer.)

If n is prime, then n is odd or n is 2.
 >[!answer]
 >Let $p=$ "n is prime", $q=$ "n is odd", and $r=$ "n is 2".
 >1. If n is prime and n is even, then n is 2.
 >2. If n is prime and n is not 2, then n is odd.
 

## 16

In 16, write each of the two statements in symbolic form and determine whether they are logically equivalent. Include a truth table with a few words of explanation to show that you understand what it means for statements to be logically equivalent.

If you paid full price, you didn't buy it at Crown Books. You didn't buy it at Crown Books or you paid full price
```ad-answer
Let $p-$ "you paid full price" and $q=$ "you bought it at Crown Books".
**Symbolic Representation of Statements:**
$$
\begin{align}
&(1)&& p\to\lnot q \\
&(2)&& \lnot q\lor p \\
\end{align}
$$
**Truth Table:**

| p | q | $\lnot q$ | $p\to\lnot q$ | $\lnot q\lor p$ |
| ---- | ---- | ---- | ---- | ---- |
| T | T | F | F | T |
| T | F | T | T | T |
| F | T | F | T | F |
| F | F | T | T | T |
Because the two statement columns in the truth table are not equivalent, the statements are **not logically equivalent.** 
```


## 20

Write negations for each of the following statements. (Assume that all variables represent fixed quantities or entities, as appropriate.)

### b

If today is New Year’s Eve, then tomorrow is January.
 >[!answer]
 >Let $p=$ "today is New Year's Eve" and $q=$ "tomorrow is January". $p\to q$.
 >$\lnot(p\to q)\equiv p\land\lnot q$, this relationship is derived in the textbook.
 >**Today is New Year's Eve and tomorrow is not January.**
### e

If x is non-negative, then x is positive or x is 0.
 ```ad-answer
 Let $p=$ "x is non-negative", $q=$ "x is positive", and $r=$ "x is 0". $p\to(q\lor r)$.
 $$
 \begin{align}
  \lnot(p\to(q\lor r))&\equiv p\land\lnot(q\lor r)&& (20b)\\
  &\equiv p\land(\lnot q\land\lnot r) && (De\ Morgan's\ Law)
  \end{align}
  $$
  **X is non-negative, X is not positive, and X is not 0. **
```
 

## 22

Write contrapositives for the statements

### b

If today is New Year’s Eve, then tomorrow is January.
 >[!answer]
 >Let $p=$ "today is New Year's Eve" and $q=$ "tomorrow is January". $p\to q$.
 >${p\to q\equiv \lnot q \to \lnot p}$.
 >If tomorrow is not January, then today is not New Year's Eve.
### e

If x is non-negative, then x is positive or x is 0.
```ad-answer
Let $p=$ "x is non-negative", $q=$ "x is positive", and $r=$ "x is 0". $p\to(q\lor r)$.
$$
\begin{align}
p\to(q\lor r)&= \lnot(q\lor r)\to \lnot p && (Given) \\
&\equiv (\lnot q\land\lnot r)\to \lnot p && (De\ Morgan's\ Law) 
\end{align}
$$
If X is not positive and X is not 0, then X is not non-negative.
```
 

## 23

Write the converse and inverse for each statement

### b

If today is New Year’s Eve, then tomorrow is January.
 >[!answer]
 >Let $p=$ "today is New Year's Eve" and $q=$ "tomorrow is January". $p\to q$.
 >**Converse:**$q\to p$
 >If tomorrow is January, then today is New Year's Eve. <br>
 >**Inverse:**$\lnot p \to \lnot q$
 >If today is not New Year's Eve, then tomorrow is not January.
### e

If x is non-negative, then x is positive or x is 0.
```ad-answer
Let $p=$ "x is non-negative", $q=$ "x is positive", and $r=$ "x is 0". $p\to(q\lor r)$.
**Converse:** $(q\lor r)\to p$
If x is positive or x is 0, then x is non-negative. <br>
**Inverse:**
$$
\begin{align}
p\to(q\lor r)&= \lnot p \to\lnot(q\lor r) && Given \\
&\equiv\lnot p \to \lnot q \land \lnot r
\end{align}
$$
If X is not non-negative, then X is not positive and X is not 0.
```


## 27

Use truth tables to establish the truth of this statement

The converse and inverse of a conditional statement are logically equivalent to each other.
 >[!answer]
 >
| p | q | $q\to p$ | $\lnot p$ | $\lnot q$ | $\lnot p\to\lnot q$ |
| ---- | ---- | ---- | ---- | ---- | ---- |
| T | T | T | F | F | T |
| T | F | T | F | T | T |
| F | T | F | T | F | F |
| F | F | T | T | T | T |
Because $q\to p$ and $\lnot p\to \lnot q$ always have the same truth values according to the table, we can conclude that the two statements are logically equivalent.


## 30

If statement forms $P$ and $Q$ are logically equivalent, then $P\iff Q$ is a tautology. Conversely, if $P\iff Q$ is a tautology, then $P$ and $Q$ are logically equivalent. Use $\iff$ to convert the logical equivalence to a tautology. Then use a truth table to verify each tautology.

$p\land (q\lor r)\equiv (p\land q)\lor(p\land r)$
 >[!answer]
 >$p\land (q\lor r)\iff (p\land q)\lor(p\land r)$
 >
| p | q | r | $q\lor r$ | $p\land(q\lor r)$ | $p\land q$ | $p\land r$ | $(p\land q)\lor(p\land r)$ |
| ---- | ---- | ---- | ---- | ---- | ---- | ---- | ---- |
| T | T | T | T | T | T | T | T |
| T | F | T | T | T | F | T | T |
| T | T | F | T | T | T | F | T |
| T | F | F | F | F | F | F | F |
| F | T | T | T | F | F | F | F |
| F | F | T | T | F | F | F | F |
| F | T | F | T | F | F | F | F |
| F | F | F | F | F | F | F | F |
The columns containing the entire statement forms are identical, proving the tautology.


## 41

Rewrite the statement in if-then form

Having two 45° angles is a sufficient condition for this triangle to be a right triangle.
 >[!answer]
 >If a triangle has two $45^\circ$ angles, then the triangle is a right triangle.


## 46

“If compound X is boiling, then its temperature must be at least 150°C.” Assuming that this statement is true, which of the following must also be true?

### c
	Let p = "compound X is boiling" and q = "temp must be at least 150 C"
Compound X will boil only if its temperature is at least 150°C.
 >[!answer]
 >The given statement can be rewritten as $p\implies q$, meaning p *only if* q. This is logically equivalent to the statement form $\lnot q\to \lnot p\equiv p\to q$. This is given in the textbook. Applied to this solution, we can conclude that  this **statement is true**.
### d

If compound X is not boiling, then its temperature is less than 150°C.
 >[!answer]
 >The given statement can be rewritten as $\lnot p\to\lnot q$. We can easily conclude here that $p\to q\not\equiv\lnot p\to \lnot q$. There are no laws that would disprove the previous statement, so the given **statement here is false**.
# 2.3
**Note:** *Column $m.n$, where n is an integer, represents premises $n$ in Column m. If n is a char C, then that column represents the conclusion.*
****
## 4

Use modus ponens or modus tollens to fill in the blanks in the argument so as to produce valid inferences.

If this graph can be colored with three colors, then it can colored with four colors. This graph cannot be colored with four colors.
 >[!answer]
 >$\therefore$ This graph cannot be colored with 3 colors.


## 9
	For problems 9 and 23, rows with all true premises are italicized
Use truth tables to determine whether the argument form is valid. Indicate which columns represent the premises and which represent the conclusion, and include a sentence explaining how the truth table supports your answer. Your explanation should show that you understand what it means for a form of argument to be valid or invalid.

$p\land q\to \lnot r$
$p\lor \lnot q$
$\lnot q\to p$
$\therefore \lnot r$
 >[!answer]
 >
| *1* | *2* | *3* | *4* | *5* | *6.1* | *7* | *8.2* | *9.3* | *10.C* |
| ---- | ---- | ---- | ---- | ---- | ---- | ---- | ---- | ---- | ---- |
| **p** | **q** | **r** | **$p\land q$** | **$\lnot r$<br>** | **$p\land q \to \lnot r$** | **$\lnot q$** | **$p\lor\lnot q$** | **$\lnot q\to p$** | **$\lnot r$** |
| T | T | T | T | F | F | F | T | T | F |
| *T *| *F* |* T* | *F* | *F* | *T* | *T* | *T* | *T* | *F* |
| T | T | F | T | T | T | F | T | T | T |
|* T* | *F* | *F* | *F* | *T* | *T* | *T* | *T* | *T *| *T* |
| F | T | T | F | F | T | F | F | T | F |
| F | F | T | F | F | T | T | T | F | F |
| F | T | F | F | T | T | F | F | T | T |
| F | F | F | F | T | T | T | T | F | T |
To determine the validity of the argument, we must look where all three premises are true and check to see if the conclusion is true as well. In the second row of truth values (omitting headers) all premises are true but the conclusion is false. This proves that the argument is invalid, despite the fourth row containing true premises and a true conclusion.

## 23

Use symbols to write the logical form of each argument, and then use a truth table to test the argument for validity. Indicate which columns represent the premises and which represent the conclusion, and include a few words of explanation showing that you understand the meaning of validity.

Oleg is a math major or Oleg is an economics major.
If Oleg is a math major, then Oleg is required to take Math 362.
$\therefore$ Oleg is an economics major or Oleg is not required to take Math 362.
```ad-answer
Let $p=$ "Oleg is a math major", $q=$ "Oleg is an econ major", and $r=$ "Oleg is required to take MATH362".
**Argument from:**
$$
\begin{align}
& p \lor q \\
& p \to r \\
\therefore\ &q\lor \lnot r 
\end{align}
$$
**Truth Table Representation:**

| 1 | 2 | 3 | 4.1 | 5.2 | 6 | 7.C |
| ---- | ---- | ---- | ---- | ---- | ---- | ---- |
| **p** | **q** | **r** | **$p\lor q$** | **$p\to r$** | **$\lnot r$** | **$q\lor\lnot r$** |
| *T* | *T* | *T* | *T* | *T* | *F* | *T* |
| *T* | *F* | *T* | *T* | *T* | *F* | *F* |
| T | T | F | T | F | T | T |
| T | F | F | T | F | T | T |
| *F* | *T* | *T* | *T* | *T* | *F* | *T* |
| F | F | T | F | T | F | F |
| *F* | *T* | *F* | *T* | *T* | *T* | *T* |
| F | F | F | F | T | T | T |
|  |  |  |  |  |  |  |
|  |  |  |  |  |  |  |
In the second row of this truth table (omitting headers), the two premises are seen to be true, yet the conclusion made is not. This leads us to the conclusion that the argument is invalid, regardless of what the rest of the truth table says.
```

## 29-32 

Some of the arguments in 29–32 are valid, whereas others exhibit the converse or the inverse error. Use symbols to write the logical form of each argument. If the argument is valid, identify the rule of inference that guarantees its validity. Otherwise, state whether the converse or the inverse error is made.

### 29

If at least one of these two numbers is divisible by 6, then the product of these two numbers is divisible by 6.
Neither of these two numbers is divisible by 6.
$\therefore$ The product of these two numbers is not divisible by 6.
```ad-answer
**Logical Form of Argument:**
Let $p=$ "At least one of the two numbers is divisible by 6" and $q=$ "The product of these two numbers is divisible by 6".
$$
\begin{align}
p&\to q \\
& \lnot p \\
\therefore\ &\lnot q
\end{align}
$$
This is the textbook definition of an inverse error. The argument is invalid.
```

### 32

If I get a Christmas bonus, I’ll buy a stereo.
If I sell my motorcycle, I’ll buy a stereo.
$\therefore$ If I get a Christmas bonus or I sell my motorcycle, then I’ll buy a stereo.
```ad-answer
**Logical Form of Argument:**
Let $p=$ "I get a Christmas bonus", $q=$ "I sell my motorcycle", and $r=$ "I'll buy a stereo".
$$
\begin{align}
p&\to r \\
q&\to r \\
\therefore\ (p\lor q)&\to r
\end{align}
$$
This can be proved with division into cases, which states that:
$$
\begin{align}
p&\land q \\
p&\to r \\
q&\to r \\
&\therefore r
\end{align}
$$
By this definition, the argument presented is confirmed to be true.
```


## 40

Sharky, a leader of the underworld, was killed by one of his own band of four henchmen. Detective Sharp interviewed the men and determined that all were lying except for one. He deduced who killed Sharky on the basis of the following statements:

1. Socko: Lefty killed Sharky.
2. Fats: Muscles didn’t kill Sharky.
3. Lefty: Muscles was shooting craps with Socko when Sharky was knocked off.
4. Muscles: Lefty didn’t kill Sharky.

Who did kill Sharky?
 >[!answer]
 >Only one of the interviewed people are telling the truth. Lefty is accusing Fats, giving Muscles and Socko an alibi. The issue with this is that if he is telling the truth, then that means that Muscles and Fats are lying which accuses both Muscles *and* Lefty. This cannot be the case, so **Lefty is lying**. If Fats is telling the truth, then that means Socko and Muscles are lying, but they are giving conflicting information, so a correct conclusion cannot be made, therefore **Fats is lying**. If Socko is telling the truth, then Fats is lying which accuses Muscles and Muscles is lying which accuses Lefty. Since two conclusions are made here, the detective could not have founf Socko to be telling the truth. **Socko is lying**. By the process of elimination, Muscles *must* be the killer, but to confirm, we must check his truth against the other lies. If he is telling the truth, then Sock is not accusing Lefty, Fats is accusing Muscles, and Lefty is not giving Muscles an alibi. Using this information we can deduce that **Muscles killed Sharky**.


## 44

A set of premises and a conclusion are given. Use the valid argument forms listed in Table 2.3.1 to deduce the conclusion from the premises, giving a reason for each step as in Example 2.3.8. Assume all variables are statement variables.

1. $p\to q$
2. $r\lor s$
3. $\lnot s\to\lnot t$
4. $\lnot q\lor s$
5. $\lnot s$
6. $\lnot p\land r\to u$
7. $w\lor t$
8. $\therefore u\land w$
```ad-answer
**Forming a Conclusion Based off of Premises and Inference Rules:**
$$
\begin{align}
&(1)&& p\to q && Premise \\
&(2)&& r\lor s && Premise \\
&(3)&& \lnot s\to \lnot t && Premise \\
&(4)&& \lnot q \lor s && Premise \\
&(5)&& \lnot s && Premise \\
&(6)&& \lnot p \land r \to u && Premise \\ 
&(7)&& w \lor t && Premise \\
&(8)&& r && Elimination\ with\ (2)\ and\ (5) \\
&(9)&& \lnot q && Elimination\ with\ (4)\ and\ (5) \\
&(10)&& \lnot p && Modus\ Tollens\ with\ (1)\ and\ (9) \\
&(11)&& \lnot t && Modus\ Ponens\ with\ (3)\ and\ (5) \\
&(12)&& \lnot p \land r && Conjuction\ with\ (10)\ and\ (8) \\
&(13)&& u && Modus\ Ponens\ with\ (6)\ and\ (12) \\
&(14)&& w && Modus\ Ponens\ with\ (7)\ and\ (11) \\
&(15)&& u\land w && Conjunction\ with\ (13)\ and\ (14) \\
&&&&\therefore u\land w
\end{align}
$$
The Conclusion derived above is identical to the one that was asked to be proven.
```
## Acknowledgements  
#### Thank you to Trevor Nichols for copying textbook questions into a markdown format. 