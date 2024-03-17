---
tags:
  - CompSci/dev/backend/container/K8s/object
aliases:
  - hpa
---
# K8s Horizontal Pod Autoscaling
### Description:
- Scales the [[K8s pod|pods]] horizontally
- `kubectl get hpa`
### behaviour:
- scaledown:
	- stabilizationWindowSeconds: helps keep a pod alive after created to prevent thrashing