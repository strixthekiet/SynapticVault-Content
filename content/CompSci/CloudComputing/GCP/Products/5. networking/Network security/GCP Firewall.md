---
tags:
  - CompSci/cloud-computing/GCP/product/NetworkSecurity
---
# GCP Firewall
### Description:
- Bidirectional
### [[Firewall]] policies:
- Stateful: means that if a connection is allowed between a source and a target or a target at a destination, all subsequent traffic in either direction will be allowed.
- Support:
	- [[Internet Control Message Protocol|ICMP]]
	- [[Remote Desktop Protocol]]
	- [[Secure Shell]]
	- [[Internet protocol suite]]
- The default network has pre-configured firewall rules that allow all instances in the network to talk with each other.
- Although firewall rules are applied to the network as a whole, connections are allowed or denied at the instance level.
- if all firewall rules in a network are deleted, there is still an implied "Deny all" ingress rule and an implied "Allow all" egress rule for the network.
- Compose of:
	- Direction of the rule: inbound are matched again ingress rule, likewise outbound
	- Source or destination:
		- for ingress: sources can be specified as part of the rule with IP address, source [[GCP tag|tags]] or a source service account
		- for egress: destinations can be specified as part of the rule with one or more ranges IP address
		- protocol and port: restriction to apply specific [[Internet protocol suite]] or port only
		- action: allow or deny
		- priority: order of priority, lower accepted first
		- Can assign certain policy to certain instances only
### Threats:
