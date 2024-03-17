---
tags:
  - CompSci/dev/backend/container/K8s
---
# kube-apiserver
### Description:
- the only component interacts with
- accept commands that view or change the state of [[K8s Cluster]]
- controls:
	- [[etcd]]
	- [[kube-scheduler]]
	- [[kube-controller-manager]]
	- [[kube-cloud-manager]]
	- [[kublet]]
		- report back to apiserver
### two