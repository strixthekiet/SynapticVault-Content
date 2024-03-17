---
tags:
  - CompSci/programming/Algorithm/Greedy
---
# Minimize Lateness Problem
### Description:
- Given a set of n jobs all of which must be scheduled on a single resource such that all jobs arrive at time $s$ and each job has a deadline $d_i$ and a length $t_i$, 
- How to minimize the maximum lateness of the resulting schedule?
	- total lateness, $\sum l_j=\sum max(0,f_i-d_j)$ 
### Earliest deadline first algorithm:
- Sort all the jobs based on deadline
- for each job
	- assign to interval
	- calculate deadline
- Why is this complete and optimal?