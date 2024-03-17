---
tags:
  - CompSci/cloud-computing/GCP/product/CloudConnectivity
---
# GCP Virtual Private Network
### Description:
- For low-volumn data connections
- Supports:
	- Site-to-site VPN
	- Static routes
	- Dynamic routes with [[GCP Router]]
- Cloud VPN tunnel:
- Cloud VPN gateway:
- Peer VPN gateway:
### Classic VPN:
- Deprecated, use HA VPN
- Encrypt and descrypt data on public internet
- Cloud VPN Gateway
	- regional resource that uses a regional external IP address
- maximum transmission unit, or **MTU, for your on-premises VPN gateway cannot be greater than 1460 bytes**.
- A VPN tunnel then connects your VPN gateways and serves as the virtual medium through which encrypted traffic is passed.
- In order to create a connection between two VPN gateways, you must establish two VPN tunnels.
- Each tunnel defines the connection from the perspective of its gateway, and traffic can only pass when the pair of tunnels is established.
