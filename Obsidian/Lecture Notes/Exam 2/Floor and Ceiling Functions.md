````ad-def
title: Floor and Ceiling Functions
#### The Floor Function:
$$
\begin{align}
\forall x\in&\mathbb{R}\text{, floor of x} \\
\lfloor{x}\rfloor&\text{ is the largest integer that is}\le x \\
\end{align}
$$
```ad-example
$\lfloor{2}\rfloor = 2$
$\lfloor{-3.5}\rfloor = -4$
```
$$
\begin{align}
\forall x\in&\mathbb{R}, \\
\lfloor{x}\rfloor \le x& < \lfloor{x}\rfloor + 1 \\
\end{align}
$$
#### The Ceiling Function:
$$
\begin{align}
\lceil{x}\rceil = \text{ smallest Integer that is }\ge x \\
\end{align}
$$
**Similarly**
$$
\begin{align}
\forall x\in& \mathbb{R} \\
\lceil{x}\rceil - 1 < x& \le \lceil{x}\rceil \\
\end{align}
$$
```ad-info
title: Generalization
$\forall x\in\mathbb{R}$
$\lceil{x}\rceil \le \lfloor{x}\rfloor + 1$
**Or if x is not an integer**
$\forall x\not\in\mathbb{Z}$
$\lceil{x}\rceil = \lfloor{x}\rfloor + 1$
```
````
#### Theorem
````ad-theory
title: Theorem 4.6.1
$$
\begin{align}
\forall x\in\mathbb{R}, m\in\mathbb{Z} \\
\lfloor{x+m}\rfloor = \lfloor{x}\rfloor + \lfloor{m}\rfloor \\
\end{align}
$$
```ad-def
title: Proof
Let $x\in\mathbb{R}$
$$
\lfloor{x}\rfloor \le x < \lfloor{x}\rfloor + 1
$$
Add m
$$
\lfloor{x}\rfloor + m \le x + m < \lfloor{x}\rfloor + m + 1
$$
$$\therefore\lfloor{x+m}\rfloor = \lfloor{x}\rfloor + m$$
```
**We can generalize and say that...**
$$
\text{If}\dots a\le b< a+ 1\qquad\text{Then}\dots a = \lfloor{b}\rfloor
$$
````
