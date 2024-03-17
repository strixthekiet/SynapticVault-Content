---
tags:
  - CompSci/dev/backend/container/K8s/CLI
---
# kubectl explain
### Description:
- List the fields for supported resources.
- Describes the fields associated with each supported API resource. 
	- Fields are identified via a simple JSONPath identifier:
	- `<type>.<fieldName>[.<fieldName>]`
### Synopis:
- `kubectl explain RESOURCE`
	- `--api-version`
	- `--recursive`
		- display all of the fields at once without descriptions. Information about each field is retrieved from the server in OpenAPI format.