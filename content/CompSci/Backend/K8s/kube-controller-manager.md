---
tags:
  - CompSci/dev/backend/container/K8s/object
---
# kube-controller-manager
### Description:
- Continuously monitors the state of a cluster thru kube-apiserver
- Do remediation when states are not met
- 
- There are many type of controllers:
	- Node controller: Responsible for noticing and responding when nodes go down.
	- Job controller: Watches for Job objects that represent one-off tasks, then creates Pods to run those tasks to completion.
	- EndpointSlice controller: Populates EndpointSlice objects (to provide a link between Services and Pods).
	- ServiceAccount controller: Create default ServiceAccounts for new namespaces.
	- ...
### two