---
tags:
  - CompSci/programming/Algorithm/Greedy
---
# Interval Scheduling Problem
### Description:
- Given a set of jobs which job $j$ starts at $s_j$ and finishes at $f_j$
- How to do the maximum of mutually compatible jobs in a given time frame
### Earliest Finish Time First Algorithm:
- $O(n\log \ n$ )
- Sort all job by the **finishing time**
- Let schedule, S, be a set of jobs
- loop thru all job:
	- if the job is compatible with S
		- add the job
- return S