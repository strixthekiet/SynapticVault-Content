---
tags:
  - CompSci/system/binary/logic-gate
---
# 4-bit Adder
### Description:
- ![](https://media.geeksforgeeks.org/wp-content/uploads/20190824181600/dig51.png)
- Made with [[1-bit Full Adder]]
- When $k$ is 0, it adds 2 numbers
### Subtraction:
- When we wish to subtract A to B, we use A + (flip bits of B) + 1
	- flip + 1 is [[Two's Complement]]
- Conveniently, when K is 1, C_in can also act as 1
- Then we use multiplexer to choose B or not B (flipped) which is B_i XOR K