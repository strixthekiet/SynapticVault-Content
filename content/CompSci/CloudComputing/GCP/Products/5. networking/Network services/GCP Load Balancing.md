---
tags:
  - CompSci/cloud-computing/GCP/product/CloudLoadBalancing
  - CompSci/network/server
aliases:
  - load balancer
---
# GCP Load Balancing:
### Description:
- [[Load balancing]]
- A load balancer is essentially a set of traffic engineering rules that are coming into the Google network, and VPC is applying your rules destined to your IP address subnet range.
- Assign an IP to the LB then fetch from that LB to use it
- instance -> disk -> image -> instance template -> instance group -> backend service+health check -> application load balancer
	- target pool? 
		- https://console.cloud.google.com/loadbalancing/advanced/targetPools/list
- Works for:
	- [[HTTP(s)]]
	- [[Secure Sockets Layer]]
	- [[UDP]]
- Provides cross-region [[Load balancing|load balancing]] including automatic failover
- applications are available to your customers at a single **anycast IP address**, which simplifies your DNS setup.
- ![|500](https://cloud.google.com/static/load-balancing/images/lb-product-tree.svg)
	- Must use passthough for preserving IP address of client
- Global load balancers:
	- Global external HTTP(s)
		- cross-regional load balancing for a web application
	- External HTTP(s) load balancing (classic)
	- External SSL proxy:
		- for Secure Sockets Layer traffic that is not HTTP
		- If it’s other TCP traffic that doesn’t use SSL
	- External TCP proxy
- 
	- Regional load balancer: to load balance UDP traffic, or traffic on any port number, you can still load balance across a Google Cloud region
	- Regional internal load balancer: load balance traffic inside your project, say, between the presentation layer and the business layer of your application
	- Google Cloud Internal HTTP(S) Load Balancing is a proxy-based, regional Layer 7 load balancer that also enables you to run and scale your services behind an internal load balancing IP address.
	- 
### Application Load Balancer (HTTP/S)
- Layer 7 load balancing for [[HTTP(s)]] application
- When a user request comes in, the load balancing service ==determines the approximate origin== of the request from the source IP address.
- Cross-region load balancing:
	- If there are no healthy instances with available capacity in a given region, the load balancer instead sends the request to the next closest region with available capacity.
- Content-based load balancing:
	- .
- HTTP(s)
	- Use target HTTP(S) proxy instead of http proxy
	- ﻿﻿Client [[Secure Sockets Layer]] session terminates at the load balancer
	- ﻿﻿Support the [[QUIC]] transport layer
	- Must create at least one SSL certificate that can be used by the target proxy for the load balancer.
		- up to 15 SSL certificates.
		- For each SSL certificate, you first create an SSL certificate resource, which contains the SSL certificate information.
		- SSL certificate resources are used only with the load balancing proxies such as a target HTTPS proxy or target SSL proxy????
1. 
	- Internet facing or internal only
	- Global vs internal
2. Front-end configuration:
	- Configure the load balancer's frontend IP address, port, and protocol. 
	- Configure an SSL certificate if using HTTPS.
	- New Frontend IP and port:
		- Protocol:
			- HTTPS requires [[Secure Sockets Layer#SSL certificate|SSL certificate]]
		- IP version
		- IP address:
			- Should have a static
		- Port:
			- 443 for HTTPS
		- Certificate (HTTPS)
3. Back-end configuration:
	- Backend services:
		- Each is 1 [[Compute Engine Managed Instance Group]]
			- can be in different region
			- Should use HTTP instead of https because its inside network
			- Can have multiple service
			- With port number
			- And balancing mode between instances
		- [[Cloud CDN]]?
		- ﻿﻿[[GCP Health Check]]
			- Pulls info at interval
			- Through [[HTTP(s)|HTTP]] so firewall must allows **130.211.0.0/22** and **35.191.0.0/16**
			- Better to use tag
		- Logging:
			- Sample of x\*100 percents
		- ﻿﻿Session affinity (optional)
			- Uses round-robin normally, can be overridden with session affinity
			- Send same request from same user to 1 instance only
		- 
		- ﻿﻿Time out setting (30-sec default)
			- fixed live timeout, not idle
	- Backend bucket:
		- for [[Google Cloud Storage]], can be used with HTTPs
		- Common use case is: send requests for dynamic content to a backend service;  static content to a backend bucket.
4. Routing rules:
	- Determine how your traffic will be directed depemds on the host and path
	- For example, some IP sends to somewhere and /video sends to different backend service
### Network Load Balancer (TCP/SSL)
- SSL proxy:
	- For encrypted non-HTTP traffic.
	- Terminates user SSL connections at the load balancing layer
		- then balancer establish new connections to backend instances using the SSL or TCP protocols.
		- SSL recommended
	- Both Ipv4 and IPv6
- TCP proxy:
	- For unencrypted, non-HTTP traffic.
	- Terminates your customer's TCP sessions at the load balancing layer
		- then forwards the traffic to your virtual machine instances using TCP or SSL.
	- Both Ipv4 and IPv6
	- 
### Network Load Balancer
- Regional
- Non-proxied, the traffic passes through the load balancer instead
- the traffic can only be balanced between VM instances that are in the same region
- 
### Network Load Balancer (UDP/Multiple protocols)
- Can use it to load balance UDP traffic and to load balance TCP and SSL traffic on ports that are not supported with the TCP proxy and SSL proxy load balancers.
- https://www.youtube.com/watch?v=Te_E_gEz14g???
- Target pool
### Internal TCP/UDP:
- Regional, private
	- Therefore you configure an internal TCP/UDP load balancing IP address to act as the front end to your private back-end instances.
- Doesnt terminate at lb, but direct it to the instance directly
### Internal HTTP(s):
- 
