# Introductory Terminology and Language
****
>[!def] Sets
>A Set is a collection of elements.
>Notation: ${2\in A, S \not\in A}$

Example: ${A = \set{1,2,T,*,CWRU}}$
#### A set is defined by its elements, Not:
1. The order of its elements 
2. Its repeated elements
>[!example] Set Equivalence
>Let ${A_1 = \set{1,2,3}, A_2 = \set{1,1,2,2,2,3},A_3 = \set{1,3,2}}$
>${A_1 = A_2=A_3}$
>Let ${A_4 = \set{1,\set{1},1}}$, Then ${A_4}$ has 2 distinct elements

The Number of distinct elements in a set can be represented by its *cardinality*
>[!def] Cardinality
>Let ${A_1 = \set{1,2,3}, A_2 = \set{1,1,2,2,2,3},A_3 = \set{1,3,2}}$ and ${A_4 = \set{1,\set{1},1}}$.
>${|A_1| = |A_2|=|A_3|=3}$ while ${|A_4| = 2}$
# Common ways to Notate Frequently Used Sets
- #### ${\mathbb{Z}}$ is the set of all integers
	${\mathbb{Z}^+}$ and ${\mathbb{Z}^-}$ represent the sets of all positive and negative integers, respectively
		*${0 \not\in (\mathbb{Z^+}\lor \mathbb{Z^-})}$*
- #### ${\mathbb{Q}}$ is the set of all rational Numbers
- #### ${\mathbb{R}}$ is the set of all real numbers
>[!note] Relation Between Common Sets
>**The three sets listed above can be compared using their cardinalities in the following manner:**
>${|\mathbb{Z}|=|\mathbb{Q}|<|\mathbb{R}|}$
>*This relation is logical because there is a countably infinite number of integers and rational numbers, but the set of all real numbers is uncountable*
## Property Base Form
>[!example] Notation
>${A_1=\set{x\in D\ |\ p(x)}}$
>${A_2=\set{z\in\mathbb{Z}\ |\ 1<x<3}=\set{2}}$
>**General Form:** ${S = \set{x\ |\ y}}$, where:
>- x denotes the general domain
>- y denotes the restriction
>- | denotes 'and'
## Subsets
![[Subsets|200]]
>[!def] Definition of a Subset
>A is a subset of B if every ${x \in A, x\in B}$
>*This is demonstrated by the above drawing*
>**Notation:** ${A \subseteq B}$ means A is a subset of B
#### If ${(A\subseteq B)\land(B\subseteq A)\to A=B}$
# Power Sets
>[!def] Definition of a Power Set
>$P(A)=$ the subset of all subsets of A
>- All Power sets contain an empty set, $\emptyset$
>*This is defined as 'the set of nothing*
#### Power Sets and Cardinality
> [!example]
> Let $A_2=\set{2,1} \therefore P(A_2)=\set{\set{1},\set{2},\set{1,2},\emptyset}$
> The following conclusions can be made: $|A_2|=2$ and $|P(A_2)=4|$
#### If $|A|=n$ then $|P(A)=2^n|$
# Cartesian Product and Coordinate Systems
	Given two elements a and b, (a,b) is an ordered pair that maps to a spot in the ab-plane
> [!def] Definition
>Given two sets $A$ and $B$, the cartesian product of $A$ and $B$ is:
>$(A \times B)=\set{(a,b)\ |\ a\in A,b\in B}$
>*If $|A|=n$ and $|B|=n$, then $|A\times B|=n \cdot n$*
>
#### It should be noted that $A\times B \not= B\times A$
```ad-example
$$
\begin{align}
(step\ 1) && A = \set{1,2}, B = \set{x,y} \\
(step\ 2) && A \times B = \set{(1,x),(1,y),(2,x),(2,y)}
\end{align}
$$
```
#### Suppose $A = B = \mathbb{R}$
- $A \times B=\mathbb{R} \times \mathbb{R}=\mathbb{R}^2$
- $\mathbb{R} \times \mathbb{R}^2=\mathbb{R}^3$
This is the basic outline for the xy-plane and coordinate system we have used for centuries