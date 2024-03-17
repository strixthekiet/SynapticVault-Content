---
tags:
  - CompSci/cloud-computing/GCP/product/CloudConnectivity
  - CompSci/network
---
# [GCP Connectivity](https://console.cloud.google.com/hybrid)
### Description:
- Allows another network to communicate thru private IP addresses

|  | Dedicated (direct to Google) | Shared (thru ISP/partner) |
| ---- | ---- | ---- |
| Layer 3 (Peering over Public IP) | [[GCP Network Peering]] | [[GCP Carrier Peering]], [[GCP Partner Interconnect]] |
| Layer 2 (Direct access with internal IP) | [[GCP Dedicated Interconnect]] | [[GCP Partner Interconnect]] |
| Over Internet | [[GCP Virtual Private Cloud]] & [[High Availability Virtual Private Network\|HA VPN]] | Public IP |
- [[Cross-cloud Interconnect]]
- Layer 3 meaning rent office in Google Pop
	- Interconnects are different from peering in that they give you connectivity using private address space into your Google VPC
- Layer 2 is thru [[Internet Service Provider]]
- ![[network-decisiontree.png]]
### 1. Network connectity center:
### 2. [[GCP Virtual Private Network]] and [[High Availability Virtual Private Network]]
### 3. Interconnect:
- Connect in very high-volumn data
- VLAN attachment:
	- Connections between your local routers and Google Cloud routers for your Dedicated or Partner Interconnect connections.
- Physical connection:
	- Establish high bandwidth, low latency connections between your Google Cloud VPC networks and your on-premises infrastructure.
- Interconnect type:
	- Typical IPsec VPN protocol:
		- Go through public internet, encypted
		- Requires On-premises VPN gateway
	- [[GCP Dedicated Interconnect]]
	- [[GCP Partner Interconnect]]
	- Cross-cloud:
		- 
### 4. Cloud routers:
- [[GCP Router]]
- Let other networks and GCP Virtual Private Cloud  exchange route information over the VPN using the [[Border Gateway Protocol]]
- Using this method, if you add a new subnet to your Google VPC, your on-premises network will automatically get routes to it.