---
tags:
  - CompSci/network/term
aliases:
  - subnetwork
  - subnet
---
# Subnet
### Description:
- Divide a network into a smaller subnetwork
### Classful subnet:
- For IPv4 only
- |Class|Leading bits|Size of network number bit field|Size of _rest_ bit field|Number of networks|Number of addresses per network|Start address|End address|
	|---|---|---|---|---|---|---|---|
	|A|0|8|24|128 (2^7)|16777216 (2^24)|0.0.0.0|126.255.255.255|
	|B|10|16|16|16384 (2^14)|65536 (2^16)|128.0.0.0|191.255.255.255|
	|C|110|24|8|2097152 (2^21)|256 (2^8)|192.0.0.0|223.255.255.255|
	|D|1110|28|2^4|2^28|224.0.0.0|239.255.255.255|
- Some chunks of it are reserved for [[RFC 1918]]
### [[Classless Inter-Domain Routing|Classless subnet]]
### Subnet mask:
- Tells which part of the IP identifies the host
	- ex: 222.222.0.0/24 means the every devices in the network has first 24 same to the host
