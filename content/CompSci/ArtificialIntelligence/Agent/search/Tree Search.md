---
tags:
  - Math/discrete/graph/tree/search
---
# Search Tree
### Description:
- Returns a solution or a failture
- Mains a [[Fringe]]
### Function:
```pseudo
function TREE-SEARCH(problem, strategy) returns a solution or failture
	initialize the search tree using the initial state of the problem
	loop do
		if there is no candidate for expansion then return failture
		choose a leaf node for expansion according to strategy
		if the node contains a goal state then return the corresponding solution
		else expand the node and add the resulting nodes to the search tree
end
```
### Searching Algorithms for tree:
- 
- Uniform search:
	- [[Depth First Search]]
	- [[Breath First Search]]
	- [[Iterative Deepening]]
	- [[Uniform Cost Search]]
- Informed search: 
	- Always have [[Heuristic Function]]
	- [[Greedy Algorithm]]
	- [[A* Search]]