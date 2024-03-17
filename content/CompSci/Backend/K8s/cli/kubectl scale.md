---
tags:
  - CompSci/dev/backend/container/K8s/CLI
---
# kubectl scale
### Description:
- [[kubectl scale]]
- Set a new size for a deployment, replica set, replication controller, or stateful set.
- Scale also allows users to specify one or more preconditions for the scale action.
- If --current-replicas or --resource-version is specified, it is validated before the scale is attempted, and it is guaranteed that the precondition holds true when the scale is sent to the server.
- `kubectl scale --current-replicas=2 --replicas=3 deployment/mysql`
### Synopsis:
- `kubectl scale`
	- `[--resource-version=version]`
	- `[--current-replicas=count]`
	- `--replicas=COUNT`
	- `(-f FILENAME | TYPE NAME)`