---
mindmap-plugin: basic
tags:
  - CompSci/dev/backend/container/K8s
aliases:
  - K8s
---
![|100](https://upload.wikimedia.org/wikipedia/commons/thumb/3/39/Kubernetes_logo_without_workmark.svg/2109px-Kubernetes_logo_without_workmark.svg.png)
# Kubernetes
# Description:
- Container orchestration engine by:
	- [[Declarative Programming|Declaratively]] state the config
	- imperatively (experienced)
- Automating deployment, scaling, and management of containerized applications.
	- goog for [[Microservice architecture]]
- The system is divided into a set of primary components that run as the [[Control Plane]] and a set of nodes that run containers.
- [Docs](https://kubernetes.io/docs/) and [Ref](https://kubernetes.io/docs/reference/)
- Frontend refers to backend [[K8s service]] so if the backend ip change, the service will update it
- [Orchestrating the Cloud with Kubernetes | Google Cloud Skills Boost](https://www.cloudskillsboost.google/course_sessions/7239637/labs/403992)
- Autoscaling: https://www.cloudskillsboost.google/course_sessions/7226348/labs/451701
# A. Documentations
# B. Getting started
# C. Concepts:
### 1. Overview:
- Objects in K8s
	- Persistent entities in the Kubernetes system.
		- Kubernetes uses these entities to represent the state of your cluster.
	- Idenfied:
		- unique name, can only have 1 object of same name at any moment
		- unique identifier, generated by k8s
	- Has:
		- Object spec: desired state
		- Object status
	- [[Kubernetes Namespaces]]
- Components:
	- ![|400](https://kubernetes.io/images/docs/components-of-kubernetes.svg)
	- [[Control Plane]]
	- [[K8s Node]]
	- Add-ons:
		- 
### 2. Cluster Architecture:
### 3. Containers:
### 4. Workloads:
- [[K8s pod]]
- Workload management:
	- [[K8s Deployment]]
	- [[K8s ReplicaSet]]
	- [[K8s StatefulSets]]
	- s
	- [[K8s CronJob]]
### 5. Service, load balancing and networking:
- [[K8s service]]:
	- Expose an application running in your cluster behind a single outward-facing endpoint, even when the workload is split across multiple backends.
- ...
- ...
### 6. Storage:
- [[K8s Volumes]]
- 
# D. Tasks:
### 1.
- 
### 6. 
### 8. Run applications:
- ...
- [[K8s Horizontal Pod Autoscaling]] vs [[K8s Vertical Pod Autoscaler]]
- ..
- [[K8s Pod Disruption Budget]]
- s
### 9. Run jobs
---
### Service:
- An abstraction which defines a logical set of Pods and a policy by which to access them.
### [[kubectl]]