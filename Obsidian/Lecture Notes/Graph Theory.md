![[Graph Theory Notes.pdf|500]]
# Euler Trails
Let G be a graph, and let v and w be two distinct vertices of G. An Euler trail from v to w is a sequence of adjacent edges and vertices that starts at v, ends at w, passes through every vertex of G at least once, and traverses every edge of G exactly once.
```ad-theory
Let G be a graph, and let v and w be two distinct vertices of G. There is an Euler trail from v to w if, and only if, G is connected, v and w have odd degree, and all other vertices of G have positive even degree.
```
# Hamiltonian Circuits
Given a graph G, a Hamiltonian circuit for G is a simple circuit that includes every vertex of G. That is, a Hamiltonian circuit for G is a sequence of adjacent vertices and distinct edges in which every vertex of G appears exactly once, except for the first and the last, which are the same
# Bipartite Graphs
Let m and n be positive integers. A complete bipartite graph on (m, n) vertices, denoted $K_{m,n}$, is a simple graph whose vertices are divided into two distinct subsets, V with m vertices and W with n vertices, in such a way that 
1. Every vertex of $K_{m,n}$ belongs to one of V or W, but no vertex belongs to both V and W
2. There is exactly one edge from each vertex of V to each vertex of W
3. There is no edge from any one vertex of V to any other vertex of V
4. There is no edge from any one vertex of W to any other vertex of W
```ad-note
title: Number of edges
For a bipartite graph $k_m$, the total number of edges is given as $m\choose2$
```
