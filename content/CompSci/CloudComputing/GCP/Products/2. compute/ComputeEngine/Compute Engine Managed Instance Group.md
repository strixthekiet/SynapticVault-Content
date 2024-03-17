---
tags:
  - CompSci/cloud-computing/GCP/product/ComputeEngine
aliases:
  - instance group
---
# Compute Engine Managed Instance Group
### Description:
- Location
	- Can select multiple zones in a region (regional) for more availability
	- Target distribution shape:
	- Instance redistribution
### 1. Instance groups:
- As same as creating an instance
- [[GCP Instance Template]] 
1. Managed instance group (stateless):
	- Autoscaling:
		- Autoscaling mode
		- Autoscaling signals:
			- Thresholds
		- Autoscaling schedules??
		- Initialization period:
			- Specify how long the VM starts before it ready to serve and do health check
	- VM instance lifecycle:
		- Action on failure:
		- Autohealing:
			- [[GCP Health Check]]
		- Updates during VM instance repair:
	- Port mapping:
		- decide whether you want to autoscale and under what circumstances and signal
2. s


- Stateless vs stateful vs
	- You can use managed instance groups for stateless serving or batch workloads. 
	- such as website front end or image processing from a queue, or for stateful applications such as databases or legacy applications.
### 2. [[GCP Health Check]]