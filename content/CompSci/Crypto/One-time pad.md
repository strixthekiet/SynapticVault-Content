---
mindmap-plugin: basic
tags:
  - CompSci/crypto
  - Math/discrete
---
# One-time pad encryption scheme
### Description:
- A private-key encryption scheme
- $M=\{0,1\}^{n}, K=\{0,1\}^n$
	- The key, $k$, is required to be as long as the message
	- The entire key used to mask the plain-text → “perfectly hides” the plain-text
### Gen:
- Generates a key $k = k_1k_2 . . . k_n$ uniformly from $K=\{0,1\}^n$
### Enc:
- $\text{Enc}_n(m_1m_2 . . . m_n) = c_1c_2 . . . c_n$, where $c_i = m_i + k_i \mod 2$ (equivalently$c_i = m_i \oplus k_i$ where $\oplus$ denotes XOR)
### Dec:
- $Dec_k (c_1c_2 . . . c_n) = m_1m_2 . . . m_n$ where $m_i = c_i − k_i \mod 2$ (it is equivalent to  $m_i = c_i \oplus k_i$)