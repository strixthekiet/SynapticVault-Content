---
tags:
  - CompSci/dev/backend/container/K8s/object
aliases:
  - vpa
---
# K8s Vertical Pod Autoscaler
### Description:
- s
	- sad
### two
- Off
- Initial
- Auto
### s
- several different recommendation types, each with values for CPU and memory: 
	- Lower Bound: this is the lower bound number VPA looks at for triggering a resize. If your pod utilization goes below this, VPA will delete the pod and scale it down. 
	- Target: this is the value VPA will use when resizing the pod. 
	- Uncapped Target: if no minimum or maximum capacity is assigned to the VPA, this will be the target utilization for VPA. 
	- Upper Bound: this is the upper bound number VPA looks at for triggering a resize. If your pod utilization goes above this, VPA will delete the pod and scale it up.