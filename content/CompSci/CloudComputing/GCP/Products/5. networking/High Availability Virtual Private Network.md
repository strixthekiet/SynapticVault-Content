---
tags:
  - CompSci/cloud-computing/GCP/product/CloudConnectivity
aliases:
  - HA VPN
---
# High Availability Virtual Private Network, HA VPN
### Description:
- High availability through an IPsec VPN connection in **a single region**.
- Must properly configure 2 or 4 [[Border Gateway Protocol|BGP]] tunnel from your ==HA VPN gateway== to your peer VPN gateway or to another HA VPN gateway.
	- HA VPN gateway can have multiple tunnels
	- Each tunnel on the 2 sides of the gateway must have the same number
- When HA VPN gateway is created, GCP automatically chooses two external IP addresses, one for each of its fixed number of two interfaces
	- from a unique address pool to support high availability.
- if you run HA VPN to a remote VPN gateway on-premises for a customer, you can connect in one of the following ways:
	- _Two on-premises VPN gateway devices:_ Each of the tunnels from each interface on the Cloud VPN gateway must be connected to its own peer gateway.
	- _A single on-premises VPN gateway device with two interfaces:_ Each of the tunnels from each interface on the Cloud VPN gateway must be connected to its own interface on the peer gateway.
	- _A single on-premises VPN gateway device with a single interface:_ Both of the tunnels from each interface on the Cloud VPN gateway must be connected to the same interface on the peer gateway.
- Depending on the way that you configure route priorities for HA VPN tunnels, you can create an active/active or active/passive routing configuration.
### Topologies:
- [HA VPN topologies  |  Google Cloud](https://cloud.google.com/network-connectivity/docs/vpn/concepts/topologies)
- 