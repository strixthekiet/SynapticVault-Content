---
tags:
  - CompSci/system/binary
---
# Two's Complement
### Description:
- Representing signed integers (both positive and negative numbers) in binary form, where the most significant bit ([[Most Significant Bit|MSB]]) signifies the sign as well as the supposed value but negative
	- ex: $1011_2=-8+2+1=-5$
### Signed extension & truncation:
- Given [[Most Significant Bit|MSB]] is 1, more $1$s added in the most left doesnt change its value. 
	- Same as  $0$
	- ex: $1011_2=111011_2=-32+16+8+2+1=5$
- But truncation will not change value if the [[Most Significant Bit|MSB]] is not 1
### Calculation:
- Much simplier than Signed integer
- Given B1+B2
- **Addition:**
	1. Convert negative numbers to their two's complement form.
	2. Perform regular binary addition.
	3. If there's an overflow (carry-out from the MSB), the result overflows and might need correction depending on the specific application.
- **Subtraction:**
	1. Negate the subtrahend (the number being subtracted) by taking its two's complement.
	2. Perform addition as described above.

