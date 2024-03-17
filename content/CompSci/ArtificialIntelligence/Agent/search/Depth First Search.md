---
tags:
  - Math/discrete/graph/tree/search
aliases:
  - DFS
---
# Depth First Search
### Description:
- Expands as much as possible of the left most node first
	- if explored go the the one to the right
	- if none left, go up 1 level
- [[Fringe]] is a [[Last In First Out Stack|LIFO stack]]
- Complete but no optimal
- Time complexity: $O(n^l)$
	- $n$ is nodes each layer 
	- $l$ for nb of layers
- Space complexity: $O(n.l)$