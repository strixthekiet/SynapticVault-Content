---
tags:
  - Math/discrete/graph
---
# Title
### Description:
- 

### 
1. Adjacency matrix:
	- A $n\times n$ matrix which has 1 at $[u][v]$ if $u$ points to $v$, otherwise 0
	- If the graph is undirected, then $a_{ij} = a_{ji}$ and the matrix 𝐴 is symmetric about the diagonal. 
		- Can be waste of memory
2. Adjacency list:
	- 1 list for each vertex and it is 1 (or the weight) if it has edge to $u$
	- $E_v=\{u|(v,u)\in E\}$
3. Edge list:
	- A list of $(u,v)$