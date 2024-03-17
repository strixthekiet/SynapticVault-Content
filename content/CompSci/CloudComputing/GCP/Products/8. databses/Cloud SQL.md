---
tags:
  - CompSci/cloud-computing/GCP/product/CloudSQL
  - CompSci/database/SQL
---
# CloudSQL
### Description:
- For [[SQL]] databases that scales ==vertically==, maximum 10230gb
- Includes:
	- [[MySQL 8.2]]
	- [[PostgreSQL]]
	- [[Microsft SQL server]]
- To automate mundane tasks like 
	- applying patches
	- updates managing backups
	- configuring replications
-  provides automated and on-demand backups with point-in-time recovery.
- Includes a network firewall
- Accessible by: 
	- Google cloud products
		- like Cloud Functions, [doc](https://cloud.google.com/sql/docs/mysql/connect-functions)
	- external services with standard MySQL driver
- `gcloud sql`
	- `gcloud sql connect my-demo --user=root --quiet`
### 0. Create
- Region and zonal availability
	- Region
	- High availability (HA):
		- within a regional instance, the configuration is made up of a primary instance and a standby instance.
		- ![|400](https://cloud.google.com/static/sql/images/ha-config.png)
		- Shared-core machines are good for prototyping, and are not covered by [Cloud SLA](https://cloud.google.com/sql/sla)
		- Each vCPU is subject to a 250 MB/s network throughput cap for peak performance. 
			- More core increases the network cap, up to a theoretical maximum of 2000 MB/s.
		- For performance-sensitive workloads such as online transaction processing (OLTP), a general guideline is to ensure that your instance has enough memory to contain the entire working set and accommodate the number of active connections.
- Customize:
	- [[#4. Connections]]
	- ..
	- 
### 1. Overview
### ...
### 4. Connections
- Summary
	- Private IP connectivity:
		- Much faster within a network with a private IP address
	- Public IP connectivity:
		- From outside of region, vpc, or even project
		- Use proxy
		- need manually control SSL certificates?
			- yes: 
				- Manual SSL Connection
				- Or Authorize networks if cant use SSL
			- No: [[Cloud SQL Auth Proxy]]
- Networkig
- Security
- Connectivity tests
### 5. Users
- s
### 6. Databases:
- 
