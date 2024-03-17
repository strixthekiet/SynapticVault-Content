---
tags:
  - CompSci/system/binary/logic-gate
aliases:
  - MUX
---
# Multiplexer
### Description:
- Selection bits decide which one is output
- Combinational circuit that has multiple data inputs and one output, along with additional control or select inputs. 
	- The control inputs determine which of the data inputs is connected to the output.
### 2-to-1 mux:
- Can be $Y=S'.A+S.b$
- ![](https://i.stack.imgur.com/VmzKJ.png)
### $2^n$-to-1 mux:
- Can be implemented with cascading 2-to-1 mux, with another selector at each higher level
- Needs $log_2(n)$ selector bits