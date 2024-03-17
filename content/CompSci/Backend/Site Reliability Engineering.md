---
tags:
  - CompSci/dev/backend
  - CompSci/network/server
aliases:
  - SRE
---
# Site Reliability Engineering, SRE
### Description:
- s
	- sad
### 4 Golden rules of Reliable server:
- Latency
- Traffic: current system demand
- Saturation: how full the service is by system capacity, percentage of utilization
- Errors: errors and fail health checks
###
- Availability, durability, and scalability are design characteristics you need to consider when developing a cloud application. 
- Availability is a measurement of uptime. Availability can be achieved through fault tolerance. You can implement backup systems in different zones or regions and use health checks to notify you when to failover to alternate resources. In Compute Engine, you can use regional or multi-regional instance groups with health checks as an option for increasing availability. 
- Durability is a measurement related to data protection. In your disaster recovery planning, durability directly relates to your recovery point objective, which is how much data you can afford to lose when a system failure happens. Important methods to improve durability include implementing a backup strategy and replicating data to multiple zones or regions depending on your needs. Implementing snapshots is a way to increase the durability of persistent disks of a Compute Engine instance. 
- Scalability defines an application’s ability to handle increased load without failing. Making an application scalable requires usage monitoring and autoscaling to respond to changes in load. Managed instance groups in Compute Engine provide autoscaling capabilities. Autoscaling in a managed instance group is based on a policy you specify. An autoscaling policy defines how the autoscaler reacts to operational needs based on instance group metrics such as average CPU, load-balancing requests per second, or specified Cloud Monitoring metrics. The autoscaler will scale in (remove instances) or scale out (add instances) based on these metrics