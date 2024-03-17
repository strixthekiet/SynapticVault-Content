---
mindmap-plugin: basic
tags:
  - CompSci/network
  - CompSci/crypto
  - Math/discrete
---
# RSA cryptosystem
### Description:
- By Ronald Rivest, Adi Shamir, Leonard Adleman
- RSA works based on modulo of the product of two large [[Prime number|primes]] $N = p · q$
- A message $m < N$ is relatively prime to $N$ (with very high probability, except for about $2/N$)
- [[Public key]] and [[Private key]] are different but mathematically linked
### Gen:
- Creation of [[Public key]] and [[Private key]]
	- Picks two random $n$-bit primes $p$ and $q$, set $N = pq$
		- This is also the private key
	- Pick a random $e$ that $1 < e < N, gcd(e, ϕ(N)) = 1$
		- $\phi(N)=(p-1)(q-1)$
	- The public key is $pk = (N, e)$
	- The private/secret key is $sk = (p, q)$ 
		- the factorization of N
	- $N$ is called the modulus of the scheme.
- Through the definition of Gen:
	- we already have a implicit definition of the [[Key space|key space]] $K$
		- The [[Message space|message space]] for a [[Public key]] is: $M_{pk} = \{m | 0 < m < N, gcd(m, N) = 1\}$
		- This happens with high probability except for $m$ is multiple of $p$ or $q$
### Enc & Dec:
- $\text{Enc}_{pk} (m) = m^{e} \mod N\to c$ 
	- Encryption using public key
- $\text{Dec}_{sk} (c) = c^{d} \mod N\to m$, 
	- where $d = e^{-1}\mod \phi(n)$
	- Decryption using private key
### Efficiency:
- Verify that all three algorithms, Gen, Enc and Dec, can be efficiently computed
- Gen involves picking two n-bit primes, $p$ and $q$, and an exponent $e$ relatively prime to $ϕ(N)$
- Enc and Dec are both modular exponentiations which can be efficiently computed.
- Dec also requires to compute $d = e ^{−1} \mod ϕ(N)$
### Correctness:
- Verify that decryption is able to recover encrypted messages. 
- Given message $0 < m < N$ and $gcd(m, N) = 1$, we have :
	- $\text{Dec}(\text{Enc}(m)) = ((m^{e} ) \mod N)^{d} \mod N$
	  $= m^{ed} \mod N$ by [[Modular arithmetic#^488f5e|modular arithmetic]] $a^{n}\mod m=(a\mod m)^n\mod m$
	  $= m^{ed \mod \phi(N)} \mod N$, by [[Euler's theorem#^d59fb0|corollary]] and $gcd(m, N) = 1$
	 $= m^{1} \mod N,$ since $d = e^{−1} \mod ϕ(N)$
	 $= m \mod N = m$ we need $0 < m < N$

### Example:
- Encrypt "STOP" with [[Public key]] (2537,13)
- Enc:
	- "STOP" -> 18 19 14 15 -> 1819 1415 so each of the block is smaller than N (2537)
	- $c=m^{13}\mod 2537\begin{cases} 1819^{13}\mod 2537 = 2081 \\ 1415^{13}\mod 2537 = 2182\end{cases}$ 
	- Encrypted message is 2081 2182
- Dec:
	- Decrypt 0981 0461 with private key is (43,59) and public
	- find $d$ by $d=e^{-1}\mod \phi(N)=13^{-1}\mod \phi(2537)\to 13d\mod 42*58=1\to d=937$ 
		- Use [[Extended Euclidean algorithm]] for $(e,\phi(N))$ so $ed+t\phi(N)=1\mod \phi N$
	- $\begin{cases} 2081^{937}\mod 2537=1819\to\text{ST}\\ 2182^{937}\mod 2537=1415\to\text{OP}\end{cases}$
### Padded RSA:
- The encryption function is deterministic. That is, once the public-key is fixed, the encryption of each message is unique!  
- Only one encryption for the word “YES”, and one encryption for the word “NO”.  
- Anyone can compute these encryptions (using the public-key) and compare with the encrypted message from Alice to Bob!  
- Solution: Alice to pad each of her message $m$ with a long random string: $m′ = (r ∥m)$
- Then encrypt padded message $m′$ as before: $(m')^{e} \mod N$

### slide 11