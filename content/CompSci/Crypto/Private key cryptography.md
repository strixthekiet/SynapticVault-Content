---
mindmap-plugin: basic
aliases:
  - Symmetric cryptography
tags:
  - CompSci/crypto
---
# Private-key cryptography
### Definition:
- A triplet of algorithms (Gen, Enc, Dec), a [[Message space|message space]] $M$, and a [[Key space|key space]] K$,$ together is called a private-key encryption scheme if:  
	1. The key-generation algorithm, Gen is a randomized algorithm that returns a key,  $k ← \text{Gen}$, such that $k ∈ K$.  
	2. The encryption algorithm, $\text{Enc}: K × M → \{0, 1\}^*$ is an algorithm that takes as input a key $k ∈ K$ and a plain-text $m ∈ M$ (the message), and outputs a cipher-text $c = \text{Enc}_k (m) ∈ \{0, 1\}^*$  
	3. The decryption algorithm, $K × \{0, 1\}^∗ → M$ is an algorithm that takes as input a key $k ∈ K$ and a cipher-text $c ∈ \{0, 1\}^*$, and output a plain-text $m ∈ M$.
	4. The scheme is correct; that is, decrypting a valid cipher-text should output the original plain text. Formally we require that for all $m ∈ M, k ∈ K,  \text{Dec}_k (\text{Enc}_k (m)) = m$
- Consists of:
	- A triplet of al algorithms [[#Gen]], [[#Enc]], [[#Dec]]
		- ```mermaid
		  flowchart LR
			subgraph Alice
			direction LR
			msg1[Message]-->ENC
			end
			ENC --jizberisz--> DEC
			subgraph Bob
			direction LR
			DEC--> msg2[Message]
			end
			sk[SecretKey]
			sk --> ENC
			sk --> DEC
	- A message space $M$
	- A key space $K$
### Algorithm triplet:
-  Gen
	- Alice and Bob first need to meet in advance to generate and agree on a [[Private key|secret key]] $k\in K$
		- Secret keys are shared
	- A uses secret key to encrypte a message, becomes a cyber text,
	- A sends cyber message to B, B then decrypt using the agreed secret key
-  Enc
	- Alice has a private message $m ∈ M$ for Bob, she sends $c = \text{Enc}_k (m)$ over the insecure channel.
-  Dec
	- Once Bob receives the cipher-text $c$, he decrypts it by running $m = \text{Dec}_k (c)$ to read the original message
### [[Caesar cipher]]
- The Caesar Cipher is a private-key encryption scheme #Math/discrete/claim 
### [[One-time pad]]
### [[Turing's code]]
- [[Known-plaintext attack]]