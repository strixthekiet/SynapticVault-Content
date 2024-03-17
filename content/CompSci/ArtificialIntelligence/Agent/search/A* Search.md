---
tags:
  - Math/discrete/graph/tree/search
  - CompSci/AI/Agent/Search
---
# A* Search
### Description:
- Order by the sum of cost in path (as in [[Uniform Cost Search|UCS]]) and the [[Heuristic Function|heuristic]] (as in [[Greedy Algorithm]])
- Expand the node with the least $f(n)=g(n)+h(n)$
	- cost so far + its heuristics
- A* is complete and optimal, provided that $h(n)$ is **admissible for tree search** and **consistent for graph search**
### Admissible heuristics:
- Inadmissible heuristic are pessimistic heuristics and break the optimality by trapping good nodes on the [[Fringe]]
- A good [[Heuristic Function|heuristic]] should be $0\le h(n)\color{tomato}\le h^*(n)$ where $h^*(n)$ is the true cost
- However, a admissible heuristic are solutions to **related problem**
	- where illegal actions are available
	- say the heuristics of going from A to B can be thru a wall
### Consistent heuristics:
- $h(s) ≤ \text{cost}(s \to n) + h(n)$ 
	- heuristic of a node is less than cost of that node to any of its neighbor and the neighbor's heuristics
	- think of it as a triangle inequality
		- ![[A* Search 2024-03-13 13.44.33.excalidraw]]
- Ensures that the first time exploring any node, it is guaranteed that that node is reached with the shortest path
---
