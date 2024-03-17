---
mindmap-plugin: basic
tags:
  - CompSci/cloud-computing
aliases:
  - vpc
  - Virtual private cloud network
  - VPN
  - Virtual private network
---
# Virtual private cloud
### Description:
- Secure, isolated private cloud hosted within a public cloud) but ==spread== among many or all regions and zones.
- Uses [[Virtual machine]]
- [[Private IP Address]] are used to communite within network, even in different region
	- The external IP address is mapped to the VM's internal address transparently by VPC.
- Traffic traveling between the two networks is encrypted by one VPN gateway, then decrypted by the other VPN gateway.
	- Uses [[IPsec]], creating a tunnel connection