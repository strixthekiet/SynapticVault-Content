---
tags:
  - CompSci/programming/Algorithm/Greedy
---
# Interval Partitioning Problem
### Description:
- Given a set of lectures which each lecture $j$ starts at $s_j$ and finishes at $f_j$
- There are rooms but each room can only facility 1 job at a time
- How to do the minimize number of rooms but all classes are possible?
- We can also observe that maximum of room is equal to the maximum depth, defined as the maximum concurrent lectures at any time.
### Earliest Finish Time First Algorithm:
- $O(n\log \ n$ )
- Sort all job by the **starting time**
- Let d be the number of room needed
- loop thru all lectures:
	- if the lecture is compatible with any classroom
		- add the lecture in that class
	- else:
		- add new classroom
		- add the lecture in that class
- return schedule