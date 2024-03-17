---
tags:
  - Math/discrete/graph/bipartite
---
# Bipartite Graph
### Description:
- A simple graph
- Its vertex set 𝑉 can be partitioned into two disjoint sets $V_1$ and $V_2$ such that every edge in the graph connects a vertex in $V_1$ and a vertex in $V_2$  
- We call the pair $(V_1,V_2)$ a **bipartition** of the vertex set 𝑉 of 𝐺.
- Some graphs that are bipartite:
	- Cycle graphs with even number of vertices
	- Every tree graph
	- Hypercube
- [[Chromatic Number]] of bipartite graph is 2
	- A graph, $G$, with atleast one edge is bipartite if and only if $\chi(G)=2$ #Math/discrete/graph/theorem 
- [[Tree]] is also a bipartite
### Theorem:
- #Math/discrete/graph/theorem 𝐺 is bipartite if and only if 𝐺 is connected and has no odd-length cycles.  
### Complete bipartite graph:
- All vertices in $V_1$ is connected to all vertices in $V_2$.
### [[Matching]] in a bipartite graph
