---
tags:
  - CompSci/cloud-computing/GCP/product/NetworkSecurity
---
# GCP NAT
### Description:
- [[Network Address Translation|NAT]]
- Let your [[Compute Engine]] instances and Kubernetes Engine container pods use Google's IP address to communicate
- NAT mapping section allows you to choose the subnets to map to the NAT gateway. 
	- You can also manually assign static IP addresses that should be used when performing NAT.
- Cloud NAT uses the [[GCP Router]] resource to group the Cloud NAT gateway configurations together. 
- Cloud NAT is not actually performed by the Cloud Router.
### Create Cloud NAT gateway
- Must have a [[GCP Router]] 
- 