---
tags:
  - Math/discrete/graph
---
# Directed graph
### Description:
- A directed graph (or digraph) $(𝑉, 𝐸)$ consists of a non-empty set of vertices $𝑉$ and a set of directed edges (or arcs) $𝐸$. 
- When (𝑢, 𝑣) is an edge of the graph 𝐺 with directed edges, 𝑢 is said to be adjacent to 𝑣 and 𝑣 is said to be adjacent from 𝑢. The vertex 𝑢 is called the initial vertex of (𝑢, 𝑣), and 𝑣 is called the terminal or end vertex of (𝑢, 𝑣). 
- The initial vertex and terminal vertex of a loop are the same.
- Types of directed graph:
	- Simple directed:
		- No loops and no multiple directed edges
	- Directed multigraph:
		- Have multiple directed edges from a vertex to a second (possibly the same) vertex
	- Multiplicity $m$:
		- When there are $m$ directed edge from $(u,v)$
	- Mixed graph:
		- When there are both undirected and directed edges
### In-degree vs out-degree:
- In-degree of a vertex 𝑣, deg$^- (𝑣)$, is the number of edges with 𝑣 as their ==terminal== vertex. 
- The out-degree of 𝑣, denoted by deg$^+(𝑣)$, is the number of edges with 𝑣 as their ==initial== vertex.
- A loop at a vertex contributes 1 to both the in-degree and the out-degree of this vertex.
- $\sum_{v\in V}\text{deg}^-(v)=\sum_{v\in V}\text{deg}^+(v)=|E|$
--