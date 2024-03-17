---
mindmap-plugin: basic
tags:
  - CompSci/cloud-computing/GCP/product/GKE
  - CompSci/dev/backend/container/K8s
aliases:
  - GKE
  - "#CompSci/cloud-computing/GCP/product/GKE"
---
![|100](https://cdn.qwiklabs.com/QKV092kALeUu8E6Qu3qVrHWJ%2BjkMkSlR%2BwZpsbfX73w%3D)
# [Kubernetes Engine](https://console.cloud.google.com/kubernetes)
### Descriptions:
- [[CaaS]], acts as a [[Control Plane]] for [[Kubernetes]]
- Google Cloud's load-balancing for [[GCP Virtual machines]]
- node pools to designate subsets of nodes within a cluster for additional flexibility
- Use [[GCP Marketplace]] for GKE templates
- In GKE, the load balancer is created as a network load balancer.
- Provide credentials
	- `gcloud container cluster get-credentials [CLUSTER_NAME] --region [REGION_NAME]`
	- only credentials for 1 cluster can be stored at a time
- `kubectl config view`
- `gcloud container clusters`
	- `gcloud container clusters create bootcamp --machine-type e2-small  --num-nodes 3 `
- Features:
	- Horitzontal Pod Autoscaler (HPA)
	- Vertical Pod Autoscaler (VPA)
	- Cluster Autoscaler (CA)
	- Node Auto Provisioning (NAP)
### Costs:
- Pay for: 
	- managed service
	- resources
	- networking
- There are a lot of add-ons, can be removed
### Google Cloud Marketplace for GKE

# A. Resource management:
### 1. Overview:

### 2. [[K8s Cluster|cluster]]
- Create Autopilot cluster:
	- auto manage:
		- **Nodes:** Automated node provisioning, scaling, and maintenance
		- **Networking:** VPC-native traffic routing for public or private clusters
		- **Security:** Shielded GKE Nodes and Workload Identity
		- **Telemetry:** Cloud Operations logging and monitoring
	- Only pays for pods, not nodes
	- No  ssh
	- no priviledge escalation
- Create Standard cluster:
	- s
### 3. Workloads
- Deployment:
	- [[Kubernetes#Deployment|K8s deployment]] 
	- Auto generate yaml file
	- Can check the events of the control plane
- Job
# B. 
