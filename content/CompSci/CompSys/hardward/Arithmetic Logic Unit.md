---
tags:
  - CompSci/system/binary/logic
aliases:
  - ALU
---
# Arithmetic Logic Unit
### Description:
- Combinational logic circuit that combines a variety of operations into a single unit.
- Has:
	- Addition/Subtraction ([[4-bit Full Adder]])
	- Logical (OR, And gates)]]
	- [[Bit Shifter]]
	- Comparisons
- Inputs: A, B and the code for OPeration
- Outputs: Y (output) and result flag
	- ![[alu.png]]
### ALU Operation Encoding in Control Logic:
- BSEL: B's selector
- LOP: logical operation
- SOP: [[Bit Shifter]] op
- OSEL: Output selector

| OP Name | OP  | BSEL | CI  | LOP | SOP | OSEL | Operation           |
| ------- | --- | ---- | --- | --- | --- | ---- | ------------------- |
| ADD     | 000 | 00   | 0   | X   | X   | 00   | Y = A + B + CI      |
| SUB     | 001 | 01   | 1   | X   | X   | 00   | Y = A + $\bar B$ +1 |
| AND     | 011 | 00   | X   | 0   | X   | 01   | Y = A and B         |
| OR      | 100 | 00   | X   | 1   | X   | 01   | Y = A OR B          |
| SHL     | 101 | X    | X   | X   | 0   | 10   | Y = A >> 1          |
| SHR     | 110 | X    | X   | X   | 1   | 10   | Y = A << 1          |
| PASS A  | 111 | 10   | 0   | X   | X   | 00   | Y = A               |