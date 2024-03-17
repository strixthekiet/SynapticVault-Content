---
tags:
  - CompSci/programming/Algorithm
---
# Coin Changing Problem
### Description:
- Given a set of demoninations of coins where there are potentially infinite number of coins for each denomination.
- How to pay the least coins possible?
### Cashier's algorithm:
- A set S of coins to return
- while x >0
	- k = largest coin such that coin value $\le$ x
	- if no k
		- return "no solution"
	- else
		- x <- x - k
		- S <- S $\cup$ k
- return S