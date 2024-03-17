---
tags:
  - CompSci/dev/backend/container/K8s/CLI
---
# kubectl get
### Description:
- Display one or many resources.
- Prints a table of the most important information about the specified resources.
	- ...
- `kubectl get pods`
### Synopsis:
- `kubectl get`
	- `[`
		- `(-o|--output=)`
			- `json|yaml|name|go-template|go-template-file|template|templatefile|jsonpath|jsonpath-as-json|jsonpath-file|custom-columns|custom-columns-file|wide`
	- `]`
	- `(`
		- `TYPE [.VERSION] [.GROUP] [NAME | -l label]`
		- `|TYPE[.VERSION][.GROUP]/NAME ...`
	- `)`
	- `[flags]`
### Flags:
- all-namespaces: -A
	- list the requested object(s) across all namespaces.
	- to get all system pods,..
