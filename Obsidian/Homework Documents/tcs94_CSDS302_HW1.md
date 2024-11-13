# **CSDS302 HW1 - Trevor Swan (*tcs94*)**
# **Section 1.2**
## Problem 3
#### a. Is $4 = \set4$?
No, because number while {4} is a set containing 4.
#### b. How many elements are in the set $\set{3, 4, 3, 5}$?
There are 3 elements in the set. 3 is repeated, but it only counts as one element.
#### c. How many elements are in the set $\set{1, \set{1}, \set{1, \set{1}}}$?
This set has 3 distinct elements, 2 of which are sets while one is a number.

## Problem 6
#### For any integer $n$, let $T_n = \set{n, n^2}$. How many elements are in each of $T_2$, $T_{-3}$, $T_1$, and $T_0$? Justify your answers.
There are 2 elements in ${T_2}$ and ${T_{-3}}$, ${T_2 = \set{2, 4}}$ and ${T_-3 = \set{-3, 9}}$. ${T_1}$ has one element, though it repeated once. ${T_0}$ is an empty set ${\set{0,0}}$ containing one element.

## Problem 7
#### Use the set-roster notation to indicate the elements in each of the following sets.
#### a. $S$ = {${{n \in \mathbb{Z} \ | \ n = (-1)^k}, for\ some\ integer \ k}$}.
${-1^1 = -1,-1^2 = 1, -1^3 = -1\  \therefore}$  ${S = \set{-1, 1}}$.
#### e. $W$ = {${s \in \mathbb{Z} \  | \  1 < t < -3}$}
${1 \lt t \lt -3}$ is not valid as ${-3 \lt 1}$.
<br><br>
#### f. $X$ = {${u \in \mathbb{Z} \ |\ u \le 4}$ $or$ ${u \ge 1}$}
${u \le 4}$ and ${u \ge 1}$ encompasses all integer values ${\therefore \ X = \mathbb{Z}}$.

## Problem 9
#### c. Is ${\set{2} \in \set{1, 2}}$?
No, ${\set{1,2}}$ contains the numbers 1 and 2, but {2} is a set ${\therefore}$ ${\set{2} \notin \set{1, 2}}$.
#### g. is ${\set{1} \subseteq \set{1, 2}}$?
Yes, ${\set{1,2}}$ contains the numbers 1 and 2, so it has the subset ${\set{1}}\therefore$ ${\set{1} \subseteq \set{1,2}}$.

## Problem 10
#### b. Is ${(5,-5) = (-5,5)}$?
No, mirrors of coordinates ${(a,b)}$ where ${a \not= b}$ are not equivalent as they amp to different regions in a plane
#### d. Is (${(\frac{-2}{-4},(-2)^3 = (\frac{3}{6}, -8)}$)?
Yes, both simplify to ${(\frac{1}{2},-8)}$.

## Problem 12
#### Let ${S = \set{2, 4, 6}}$ and ${T = \set{1, 3, 5}}$. Use the set roster notation to write each of the following sets, and indicate the number of elements that are in each set.
#### a. ${S\ X\ T}$
${= \set{(2,1), (2,3), (2,5), (4,1), (4,3), (4,5), (6,1), (6,3), (6,5)}}$
#### c. ${S\ X\ S}$
${= \set{(2,2), (2,4), (2,6), (4,2), (4,4), (4,6), (6,2), (6,4), (6,6)}}$
<br><br><br><br>
# **Section 1.3**
## Problem 2
#### Let ${C = D = \set{-3, -2, -1, 1, 2, 3}}$ and define a relation S from C to D as follows. For every ${(x,y) \in C\ X\ D, (x,y) \in S}$ means that ${\frac{1}{x} - \frac{1}{y}}$ is an integer.
#### a. Is ${2\ S\ 2}$? Is ${-1\ S\ \mathbb{-}1}$? Is ${(3,3) \in S}$? Is ${(3,-3) \in S}$?
${(2,2):\frac{1}{2}-\frac{1}{2} = 0\in \mathbb{Z}}$, yes
${(-1,-1):\frac{1}{-1}-\frac{1}{-1} = 0\in \mathbb{Z}}$, yes
${(3,3):\frac{1}{3}-\frac{1}{3} = 0\in \mathbb{Z}}$, yes
${(3,-3):\frac{1}{3}-\frac{1}{-3} = \frac{2}{3}\notin \mathbb{Z}}$, no
#### b. Write ${S}$ as a set of ordered pairs.
${(x,y)\in C\ X\ D \therefore S =}$ 
${\set{(-3,-3),\ (-2,-2),\ (-1,-1),\ (1,1),\ (2,2),\ (3,3),\ (-2,-2),\ (2,-2),\ (1,-1),\ (-1,1)}}$ 
#### c. Write the domain and co-domain of ${S}$.
Domain: ${\set{-3, -2, -1, 1, 2, 3}}$
Co-domain: ${\set{-3, -2, -1, 1, 2, 3}}$
<br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br>
#### d. Draw an arrow diagram for ${S}$.
``` dot
digraph A {
	rankdir = LR; 
	subgraph cluster_0 {
		label = "Domain"
		style="filled,rounded";
			color=lightgrey;
			node [style=filled,color=white];
			fontname="Times New Roman Bold";
				A [label="-3"];
			    B [label="-2"];
			    C [label="-1"];
			    D [label="1"];
			    E [label="2"];
			    F [label="3"];
	    }
	subgraph cluster_1 {
	    label = "Co-domain"
		style="filled,rounded";
			color=lightgrey;
			node [style=filled,color=white];
			fontname="Times New Roman Bold";
			    G [label="-3"];
			    H [label="-2"];
			    I [label="-1"];
			    J [label="1"];
			    K [label="2"];
			    L [label="3"];
	    }
		A -> G
		B -> {H, K}
		C -> {I, J}
		D-> {I, J}
		E -> {H, K}
		F -> L
}
```

## Problem 8
#### Let ${A = \set{2,4}}$ and ${B = \set{1,3,5}}$ and define relations U, V, and W from A to B as follows: 
##### For every ${(x,y) \in A\ X\ B}$
- ###### ${(x,y) \in U}$ means that ${y-x > 2}$
- ###### ${(x,y) \in V}$ means that ${y-1 = \frac{x}{2}}$
- ###### ${W = \set{(2,5),(4,1),(2,3)}}$
 <br><br>
#### a. Draw Arrow Diagrams for U, V, and W.
${A = \set{2,4}}$ and ${B = \set{1, 3, 5}}$
**For Relation U:** ${y-x>2 \therefore R_U = \set{(2,5)}}$. 
```dot
digraph A{
	rankdir = LR;
	subgraph cluster_A {
	label = "Relation U";
	style = "rounded";
	pos = "0,0!";
		subgraph cluster_0 {
		label = "Domain";
		style = "filled,rounded";
			color = lightgrey;
			node [style = filled,color = white];
			fontname = "Times New Roman Bold";
				A [label = "2",pos = "0,0!"];
				B [label = "4",pos = "0,1!"];
			}
		subgraph cluster_1 {
		label = "Co-domain";
		style = "filled, rounded";
			color = lightgrey;
			node [style = filled, color = white];
			fontname = "Times New Roman Bold";
				C [label = "1",pos = "1,0!"];
				D [label = "3",pos = "1,1!"];
				E [label = "5",pos = "1,2!"];
			}
			A -> E;
			A -> {C, D} [style = invis]
			B -> {E, C, D} [style = invis]
		}
	}
```
**For Relation V:** ${y-1>\frac{x}{2} \therefore R_V = \set{(4,3)}}$. 
```dot
digraph B {
	rankdir = LR;
	subgraph cluster_B {
	label = "Relation V";
	style = "rounded";
	pos = "0,1!";
		subgraph cluster_2 {
		label = "Domain";
		style = "filled,rounded";
			color = lightgrey;
			node [style = filled,color = white];
			fontname = "Times New Roman Bold";
				F [label = "2"];
				G [label = "4"];
			}
		subgraph cluster_3 {
		label = "Co-domain";
		style = "filled, rounded";
			color = lightgrey;
			node [style = filled, color = white];
			fontname = "Times New Roman Bold";
				H [label = "1"];
				I [label = "3"];
				J [label = "5"];
			}
			G -> I;
			G -> {I, J} [style = invis];
			F -> {H, I, J} [style = invis];
		}
	}
```
<br><br><br><br>
**For Relation W:** ${\set{(2,5),(4,1),(2,3)}}$. 
```dot
digraph C {
	rankdir = LR;
	subgraph cluster_C {
	label = "Relation W";
	style = "rounded";
	pos = "0,2!";
		subgraph cluster_4 {
		label = "Domain";
		style = "filled,rounded";
			color = lightgrey;
			node [style = filled,color = white];
			fontname = "Times New Roman Bold";
				K [label = "2"];
				L [label = "4"];
			}
		subgraph cluster_5 {
		label = "Co-domain";
		style = "filled, rounded";
			color = lightgrey;
			node [style = filled, color = white];
			fontname = "Times New Roman Bold";
				M [label = "1"];
				N [label = "3"];
				O [label = "5"];
			}
			K -> {N, O};
			L -> M;
		}
}
```
#### b. Indicate whether any of the relations U, V, and W are functions.
Functions require the elements of the domain to be mapped to an element in the co-domain. Relations U and V are not functions because they violate this rule. W is not a function because the element 2 has two mapped elements, ${\set{(2,3),(2,5)}}$.
<br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br>
## Problem 13
#### Let ${A = \set{-1, 0, 1}}$ and ${B = \set{t, u, v, w}}$. Define a function ${F:A \rightarrow B}$ by the following arrow diagram:
```dot
digraph A{
rankdir = LR;
	style = "rounded";
	pos = "0,0!";
		subgraph cluster_0 {
		label = "A";
		style = "filled,rounded";
			color = lightgrey;
			node [style = filled,color = white];
			fontname = "Times New Roman Bold";
				A [label = "-1"];
				B [label = "0"];
				C [label = "1"]
			}
		subgraph cluster_1 {
		label = "B";
		style = "filled, rounded";
			color = lightgrey;
			node [style = filled, color = white];
			fontname = "Times New Roman Bold";
				D [label = "t"];
				E [label = "u"];
				F [label = "v"];
				G [label = "w"];
			}
			A -> E;
			C -> E;
			B -> G;
	}
```
#### a. Write the domain and co-domain of F.
Domain = ${\set{-1,0,1}}$
Co-domain = ${\set{t,u,v,w}}$
#### b. Find ${F(-1), F(0)}$ and ${F(1)}$.
By the arrow diagram, we can see that ${F(-1) = u, F(0) = w}$ and ${F(1) = u}$. The input of F represents the preimage to a corresponding image.
<br><br><br><br><br><br><br><br><br><br><br>
## Problem 14
#### Let ${C = \set{1,2,3,4}}$ and ${D = \set{a,b,c,d}}$. Define a function ${G: C \rightarrow D}$ by the following arrow diagram: 
```dot
digraph A{
rankdir = LR;
	style = "rounded";
	pos = "0,0!";
		subgraph cluster_0 {
		style = "filled,rounded";
			color = lightgrey;
			node [style = filled,color = white];
			fontname = "Times New Roman Bold";
				A [label = "1"];
				B [label = "2"];
				C [label = "3"];
				D [label = "4"]
			}
		subgraph cluster_1 {
		style = "filled, rounded";
			color = lightgrey;
			node [style = filled, color = white];
			fontname = "Times New Roman Bold";
				E [label = "a"];
				F [label = "b"];
				G [label = "c"];
				H [label = "d"];
			}
			{A, B, C, D} -> G;
	}
```
#### a. Write the domain and co-domain of G.
Domain = ${\set{1,2,3,4}}$
Co-domain = ${\set{a, b, c, d}}$
#### b. Find ${G(1), G(2), G(3),}$ and ${G(4)}$.
All elements of the domain are mapped to the same element in the co-domain ${\therefore G(1) = G(2) = G(3) = G(4) = c}$.
<br><br><br><br><br><br><br><br><br><br>
## Problem 15
#### Let ${X = \set{2,3,5}}$ and ${Y = \set{1,2,4,6}}$. Which of the following arrow diagrams determine functions from X to Y.
#### d.
```dot
digraph A{
rankdir = LR;
	style = "rounded";
	pos = "0,0!";
		subgraph cluster_0 {
		label = "X";
		style = "filled,rounded";
			color = lightgrey;
			node [style = filled,color = white];
			fontname = "Times New Roman Bold";
				A [label = "2"];
				B [label = "4"];
				C [label = "5"]
			}
		subgraph cluster_1 {
		label = "Y";
		style = "filled, rounded";
			color = lightgrey;
			node [style = filled, color = white];
			fontname = "Times New Roman Bold";
				D [label = "1"];
				E [label = "2"];
				F [label = "4"];
				G [label = "6"];
			}
			A -> G;
			{B, C} -> E;
			A -> D [style = invis];
			B -> {F, G} [style = invis];
	}
```
Yes, all elements in x have one corresponding element in Y.
#### e.
```dot
digraph A{
rankdir = LR;
	style = "rounded";
	pos = "0,0!";
		subgraph cluster_0 {
		label = "X";
		style = "filled,rounded";
			color = lightgrey;
			node [style = filled,color = white];
			fontname = "Times New Roman Bold";
				A [label = "2"];
				B [label = "4"];
				C [label = "5"]
			}
		subgraph cluster_1 {
		label = "Y";
		style = "filled, rounded";
			color = lightgrey;
			node [style = filled, color = white];
			fontname = "Times New Roman Bold";
				D [label = "1"];
				E [label = "2"];
				F [label = "4"];
				G [label = "6"];
			}
			B -> E;
			C -> F;
	}
```
No, not all of the elements in X are mapped to an element in Y.

## Problem 18
#### Let ${h}$ be the constant function defined in example ${1.3.6}$. Find ${h(-\frac{12}{5}), h(\frac{0}{1})}$ and ${h(\frac{9}{17})}$.
- #### In ${1.3.6}$ the constant function is defined as ${h(r) = 2}$.
${h:r \rightarrow 2 \therefore h(\frac{-12}{5})=h(\frac{0}{1})=h(\frac{0}{1})=2}$.

## Problem 20
#### Define functions ${H}$ and ${K}$ from ${R}$ to ${R}$ by the following formulas: 
- #### For every ${x \in R, H(x) = (x-2)^2}$ and ${K(x) = (x-1)(x-3) + 1}$
#### Does ${H = K}$? Explain.
${H(x)=(x-2)^2\ \ \overrightarrow{algebraic}\ \ H(x)=x^2-4x+4}$
${K(x) = (x-1)(x-3) + 1\ \ \overrightarrow{FOIL}\ \ K(x)=x^2-3x-x+3+1\ \ \overrightarrow{simplify}\ \ K(x)=x^2-4x+4}$
H and K both simplify/expand out to be the same function, and since they have the same domain ${x \in \mathbb{R}}$ and co-domain ${(x-2)^2,H=K}$ as they are the same function.
<br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br><br>
# Section 7.1
## Problem 2
#### Let ${X = \set{1,3,5}}$ and ${Y = {Y = \set{a,b,c,d}}}$. Define ${g:X\rightarrow Y}$ by the following arrow diagram:
```dot
digraph A{
rankdir = LR;
	style = "rounded";
	pos = "0,0!";
		subgraph cluster_0 {
		label = "X";
		style = "filled,rounded";
			color = lightgrey;
			node [style = filled,color = white];
			fontname = "Times New Roman Bold";
				A [label = "1"];
				B [label = "3"];
				C [label = "5"]
			}
		subgraph cluster_1 {
		label = "Y";
		style = "filled, rounded";
			color = lightgrey;
			node [style = filled, color = white];
			fontname = "Times New Roman Bold";
				D [label = "a"];
				E [label = "b"];
				F [label = "c"];
				G [label = "d"];
			}
			{A,B,C} -> E;
			label = "Function g";
			labelloc = "t";
			fontname = "Times New Roman Bold";
	} 
```
#### a.
Domain = ${\set{1,3,5}}$
Co-domain = ${\set{a,b,c,d}}$
#### b.
All elements in the domain map to the same element in the co-domain ${\therefore g(1)=g(3}=g(5)=b$.
#### c.
Their is only one mapped image and it is ${b \therefore}$ Range = ${\set{b}}$.
#### d.
3 is an inverse image of b, not a.
1 is an inverse image of b, as b is the image of 1.
#### e.
${\set{1,3,5}}$ is the inverse image of b.
c has no inverse as there is no preimage that corresponds to c. ${\set{0}}$
#### f.
${\set{(1,b),(3,b),(5,b)}}$

## Problem 4
#### b. Find all functions from ${X = \set{a,b,c}}$ to ${Y = \set{u}}$.
There is only one function ${f(X)=Y}$ because there is only one element in the co-domain.
This function can be defined as: ${x \in X, F(x) = u}$.

# Section 7.2
## Problem 7
#### Let ${X = \set{a,b,c,d}}$ and ${Y = \set{e,f,g}}$. Define function ${G}$ by the arrow diagram below.
```dot
digraph A{
rankdir = LR;
	style = "rounded";
	pos = "0,0!";
		subgraph cluster_0 {
		style = "filled,rounded";
		label = "X: Domain of G";
			color = lightgrey;
			node [style = filled,color = white];
			fontname = "Times New Roman Bold";
				A [label = "a"];
				B [label = "b"];
				C [label = "c"];
				D [label = "d"]
			}
		subgraph cluster_1 {
		style = "filled, rounded";
		label = "Y: Co-domain of G";
			color = lightgrey;
			node [style = filled, color = white];
			fontname = "Times New Roman Bold";
				E [label = "e"];
				F [label = "f"];
				G [label = "g"];
			}
			{A, B, D} -> F;
			C -> E;
			A -> G [style=invis];
	}
```
<br><br>
#### b. Is ${G}$ one-to-one? Why or why not? Is it onto? Why or why not?
${a}$ and ${b}$ have the same image and ${a \not= b}$, so it is not one-to-one. g does not have a pre-image, so the function is not onto either.

## Problem 8
#### Let ${X = \set{a,b,c}}$ and ${Y = \set{d,e,f,g}}$. Define function ${H}$ and ${K}$ by the arrow diagrams below.
#### a. Is ${H}$ one-to-one? Why or why not? Is it onto? Why or why not?
```dot
digraph A{
rankdir = LR;
	style = "rounded";
	pos = "0,0!";
		subgraph cluster_0 {
		label = "X: Domain of H";
		style = "filled,rounded";
			color = lightgrey;
			node [style = filled,color = white];
			fontname = "Times New Roman Bold";
				A [label = "a"];
				B [label = "b"];
				C [label = "c"]
			}
		subgraph cluster_1 {
		label = "Y: Co-domain of H";
		style = "filled, rounded";
			color = lightgrey;
			node [style = filled, color = white];
			fontname = "Times New Roman Bold";
				D [label = "d"];
				E [label = "e"];
				F [label = "f"];
				G [label = "g"];
			}
			A -> D;
			{B, C} -> F;
			label = "Function H";
			labelloc = "t";
			fontname = "Times New Roman Bold";
	} 
```
${b}$ and ${c}$ have the same image, but ${b \not= c}$, so ${H}$ is not one-to-one. ${g}$ does not have a pre-image, so the function is not onto.
<br><br><br><br><br><br><br><br><br>
#### b. Is ${K}$ one-to-one? Why or why not? Is it onto? Why or why not?
```dot
digraph A{
rankdir = LR;
	style = "rounded";
	pos = "0,0!";
		subgraph cluster_0 {
		label = "X: Domain of K";
		style = "filled,rounded";
			color = lightgrey;
			node [style = filled,color = white];
			fontname = "Times New Roman Bold";
				A [label = "a"];
				B [label = "b"];
				C [label = "c"]
			}
		subgraph cluster_1 {
		label = "Y: Co-domain of K";
		style = "filled, rounded";
			color = lightgrey;
			node [style = filled, color = white];
			fontname = "Times New Roman Bold";
				D [label = "d"];
				E [label = "e"];
				F [label = "f"];
				G [label = "g"];
			}
			A -> F;
			B -> D;
			C -> E;
			label = "Function K";
			labelloc = "t";
			fontname = "Times New Roman Bold";
	} 
```
${a,b}$ and ${c}$ all have their own image, so ${K}$ is one-to-one. ${g}$ has no pre-image, so ${K}$ is not onto.