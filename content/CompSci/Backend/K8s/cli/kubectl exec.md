---
tags:
  - CompSci/dev/backend/container/K8s/CLI
---
# kubectl exec
### Description:
- Execute a command inside a [[Container]] and view the result
- `kubectl exe -it [POD_NAME]] --/bin/bash` for interactive shell to work in the container
### Synopsis:
- `kubectl exec`
	- `(`
		- `POD`
		- `| TYPE/NAME`
	- `)` 
	- `[-c CONTAINER]`
	- `[flags]`
	- `-- COMMAND [args...]`