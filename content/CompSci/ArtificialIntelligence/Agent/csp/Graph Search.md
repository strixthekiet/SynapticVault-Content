---
tags:
  - CompSci/AI/Agent/Search
---
# Search Graph
### Description:
- Like tree search but do not visit a node twice as there might be a loop
### Searching Algorithms for graph:
- Never expand a state twice
- Use any algorithm of [[Tree Search]] and a set of expanded state ("closed set")
- Before expanding a node, make sure it was not expanded before
- For [[A* Search]], heuristics must be [[A* Search#Consistent heuristics|Consistent heuristics]]