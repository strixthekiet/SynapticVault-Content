---
mindmap-plugin: basic
tags:
  - CompSci/cloud-computing/GCP/product/CloudIAM
aliases:
  - role
---
# GCP Role
### Description:
- A collection of resources permissions
	- ![|400](https://cloud.google.com/static/iam/img/role-and-permissions.svg)
	- Permissions determine what operations are allowed on a resource. 
		- They are method of classes of the API
### Types of role:
- Basic roles:
	- Defaul by Google
	- very broad
	- Includes: Owner, editor, viewer, billing admisnistrator
- Predefined role
	- Default role that has set of permissions group by service
		- For example, Compute Admin has full control over Compute Engine resources
- Custom role:
	- More fine-grained, for ex: can turn on, turn off, get list of instances but nth else on that service
	- Can select other roles to group them to new role
---
