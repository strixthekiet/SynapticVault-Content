---
tags:
  - CompSci/network/term
aliases:
  - NEG
---
# Network Endpoint Group, NEG
### Description:
- A configuration object that specifies a group of backend endpoints or services.
- A collection of IP addresses that you can apply networking functions to, like load balancing, firewalls and logging. 
	- If you're creating an HTTP(S) load balancer with backend containers, your NEG will be created automatically.
- Defines how endpoints should be reached, whether they are reachable, and where they are located.
### Types of NEG:
- Zonal and internet NEGs define how endpoints should be reached, whether they are reachable, and where they are located.
- 
- A **zonal** NEG contains one or more endpoints that can be Compute Engine VMs or services running on the VMs.
	- Each endpoint is specified by either an IP address or an IP:port combination.
- An **Internet** NEG contains a single endpoint that is hosted outside of Google Cloud.
	- This endpoint is specified by hostname FQDN:port or IP:port.
- A **hybrid** connectivity NEG points to Traffic Director services running outside of Google Cloud.
- A **serverless** NEG points to Cloud Run, App Engine, Cloud Functions services residing in the same region as the NEG.
	- Serverless NEGs don't contain endpoints.