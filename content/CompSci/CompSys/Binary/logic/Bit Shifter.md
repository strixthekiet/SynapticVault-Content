---
tags:
  - CompSci/system/binary/logic/shifter
---
# Bit Shifter
### Description:
- 
	- sad
### Logical Shifter:
- fills the empty space with 0
- Shift left: A >> 2
- Shift right: A << 2
### Arithmetic Shifter:
- Fill the empty space with the most MSB
- Shift left: 11001 >> 2 = 11110
	- In two's complement, if it negative, it keeps the same value by adding 1; if possible, add 0 in front
- shift right: 11001 << 2 = 00100
	- add 0 from the back
### Rotator Shifter:
- Rotate like a queue
	- ![](https://i.stack.imgur.com/C94CB.png)
- The selector decides how many bits are shifted and which bit to replace it
- Can be used as multiplier and divider