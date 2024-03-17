---
tags:
  - CompSci/crypto
  - Math/discrete
aliases:
  - Caesar cipher
---
# Caesar cipher
### Description:
- The Caesar Cipher is a private-key encryption scheme 
- used by Julius Caesar (100 BC-44 BC) to communicate with his generals
- encryption is achieved by “shifting” each alphabet by some fixed amount (the key).  
- Let [[Message space|message space]] $M = {A, B, . . . , Z }^*$ and key space $K = {0, 1, . . . , 25}$
### Gen:
- a uniformly random key $k$ from $K = {0, 1, . . . , 25}$
### Enc:
- Encryption shifts the alphabet of each letter in the plain-text by $k$: $\text{Enc}_k (m_{1}m_{2} . . . m_{n}) = c_{1}c_{2} . . . c_{n}, \text{ where } c_i = m_i + k \mod 26$ 
### Dec:
- Decryption shifts each letter back:  $\text{Dec}_k (c_1c_2 . . . c_n) = m_1m_2 . . . m_n, \text{ where } m_i = c_i − k \mod 26$
