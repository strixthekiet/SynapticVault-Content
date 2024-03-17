---
tags:
  - Math/discrete/graph/tree/search
aliases:
  - UCS
  - Djiktra Algorithm
---
# Uniform Cost Search
### Description:
- Expand a cheapest node first
- And organize the nodes as if the cost to reach are their depth
- [[Fringe]] is a [[Priority Queue]]
- Time complexity, $O(b^{C^*/\epsilon})$
- Space complicity, $O(b^{C^*/\epsilon})$
### Cost contour:
- ![](https://www.cs.cmu.edu/~15281/coursenotes/search/images/UCStiers.png)