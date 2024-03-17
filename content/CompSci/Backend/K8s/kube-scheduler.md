---
tags:
  - CompSci/dev/backend/container/K8s/object
---
# kube-scheduler
### Description:
- Schedule [[K8s pod|pods]] onto the [[K8s Node]]
	- when a pod doesnt have a node, it writes the of the node into the pod object
		- Doesnt launch the pod to node
	- Evaluates the requirements of each individual [[K8s pod|pod]] and select which node to deploy to
- Knows the state of all nodes
- Can define affinity parameters
	- when a group of pods should run on a same node
	- or anti-affinity
### two