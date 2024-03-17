---
mindmap-plugin: basic
tags:
  - CompSci/crypto
  - Math/discrete
---
# Turing code
### Description:
- From Alan Turing
### Version 1
- Replace each letter of a message with two digits: A = 01, B = 02, C = 03, . . . , Z = 26. 
	- For example, “victory” is translated to 22 09 03 20 15 18 25.
- Adding (a few) number to make it prime, i.e., 22 09 03 20 15 18 25 13.
- Beforehand Sender and Receiver agree on a secret key, a prime $k$.
- Encryption The sender encrypts: $\hat m = m · k$
- Decryption The receiver decrypts: $m = \hat m/k$
- However, If attack got 2 messages, they can find $gcd(\hat m_{1}, \hat m_{2})$ to have $k$
### Version 2
- Beforehand: Sender and Receiver agree on a large prime $n$, which can be public, and a [[Private key|secret key]], a prime $k < n$.
- Encryption: The sender encrypts a message $m < n$, which is a large prime: $\hat m = m \cdot_{n} k$
- Decryption: The receiver know both $n$ and $k$, so can compute $j$, an [[Prime number#^d91a8b|inverse]] of $k$ modulo $n$, and decrypts: $j \cdot_{n} \hat m = j \cdot_{n} k \cdot_{n} m = m\ (\text{as } m < n)$
- Problem:
	- if the attacker know both encrypted and unencrypted message, i.e., $m$ and $\hat m = m \cdot_{n} k$
	- Attacker can compute $j$, an inverse of $m$ modulo $n$
	- Then compute $j ·_{n} \hat m = j ·_{n} m ·_{n} k = k$
---