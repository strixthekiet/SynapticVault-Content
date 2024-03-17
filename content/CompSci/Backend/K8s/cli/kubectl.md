---
tags:
  - CompSci/dev/backend/container/K8s/CLI
---
# kubectl
### Description:
- [Doc](https://kubernetes.io/docs/reference/generated/kubectl/kubectl-commands) and [Cheatsheet](https://kubernetes.io/docs/reference/kubectl/cheatsheet/)
- Transform CLI command to and back of [[kube-apiserver]]'s api HTTPS call to control clusters
	- to authenticate incoming requests
	- and authorization
	- manage admission control
- Auth with location and credentials
- Must be configured to store credentials for each sluster
	- stored in config file in `$HOME/.kube/config` 
- `kubectl help`
### Synopis:
- `kubectl [command] [TYPE] [NAME] [flags]`
	- Types = [Resourse types](https://kubernetes.io/docs/reference/kubectl/#resource-types)
		- Use `kubectl api-resources` for a complete list of supported resources.
	- `-c` argument to specify which container
### 1. Getting started:
- [[kubectl create]]
- **[[kubectl get]]**
- [[kubectl expose]]
- [[kubectl run]]
- scale
### 2. App management:
- [[kubectl apply]]
- ...
- [[kubectl autoscale]]
- ..
- [[kubectl scale]]
### 3. Working with apps:
- [[kubectl cp]]
- **[[kubectl describe]]**
- **[[kubectl exec]]**
- **[[kubectl logs]]**
- .
- [[kubectl top]]
### 4. Cluster management:
- s
- [[kubectl cluster-info]]
- [[kubectl cordon]]
- [[kubectl drain]]
### 5. Kubectl setting and usage:
- [[kubectl config]]
- [[kubectl explain]]

