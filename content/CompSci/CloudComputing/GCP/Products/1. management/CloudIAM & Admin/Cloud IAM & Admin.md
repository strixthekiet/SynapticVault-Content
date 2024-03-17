---
tags:
  - CompSci/cloud-computing/GCP/product/CloudIAM
  - CompSci/network/security
aliases:
  - "#CompSci/cloud-computing/GCP/product/CloudIAM"
---
# [Cloud IAM & Admin](https://console.cloud.google.com/iam-admin)
### Descriptions:
- [[Identity and Access Management]]
- The **allow policy** is a collection of role bindings that bind one or more principals to individual roles. 
- When you want to define **who** ([[GCP Principal|principal]]) has what type of access ([[GCP Role|role]]) on a resource, you create an allow policy and attach it to the resource.
- Practices:
	- Use projects to group resources that share the same trust boundary.
	- ﻿﻿Check the policy granted on each resource and make sure you understand the inheritance.
	- ﻿﻿Use "principles of least privilege" when granting roles.
	- Assign VM to a custom service account that give it minimal access
	- ﻿﻿Audit policies in Cloud Audit Logs: setiampolicy.
	- ﻿﻿Audit membership of groups used in policies
- Resource hierachy in GCP are inherited from top to bottom:
	- ![|400](https://cloud.google.com/static/iam/img/policy-inheritance.svg)
- [[GCP Organization]]
- [[GCP Member]]
### 0. Resources:
- Billing is accumulated from the bottom up, as we can see on the right.
- Resource consumption is measured in quantities like rate of use or time, number of items, or feature use.
- Because a resource belongs to only one project, a project accumulates the consumption of all its resources.
- Each project is associated with one billing account, which means that an organization contains all billing accounts.
- 
- Images, snapshots, and networks, are **global resources**.
- External IP addresses are regional resources, and instances and disks are **zonal resources**
### 1. IAM policy:
- Set on the resources itself
- When you grant a [[GCP Role|role]] to a [[GCP Principal|principal]], you grant all the permissions that the role contains.
	- ![|400](https://cloud.google.com/static/iam/img/iam-overview-basics.svg)
- IAM allow vs deny policies:
	- Allow policies:
		- Some services support granting IAM permissions at a granularity finer than the project level, at the bucket level
		- By pass the role and always allow a principle from the side of the resouce
	- Deny policies:
		- Override allow policies and their role, deny from the side of a resource
- Resource policies are a union of parent and resource, where a less restrictive parent policy will always override a more restrictive resource policy.
- You can grant IAM permissions at the project level. 
	- The permissions are then inherited by all resources within that project.
- Use [[Principle of least privilege]]
### 2. Identity & Organization:
- [[GCP Identity Platform]]
### 3. 
### 4. Policies analyzer:
- ML-based findings about permission usage in your project, folder, or organization.
### 5. Organization policies:
- A configuration of restrictions, defined by configuring a constraint with the desired restrictions for that organization.
- Can be applied to the organization node, and all of its folders or projects within that node.
### 6. [[GCP Service Account]]
### 7. 
### 9. Labels:
- For more granular control than project and folder
- Key value pairs that you can attach to all types of resources
	- Each resource can have up to 64 labels.
- For example, you could create a label to define the environment of your virtual machines.
	- Then, you define the label for each of your instances as either production or test.
	- Can later search and list all of your production resources for inventory purposes.
### 10. [[GCP tag]]
### 14. [[GCP Role]]
### 15. [[GCP Audit Log]]
### 18. Quotas:
- Categories:
	- How many resources can be created per project?
	- How quickly can API request be made?
	- How many resources can be created per region
- Can ask for more quotas limit

### Access transparency logs:
- Access transparency logs help by providing logs of accesses to your data by human Googlers.
- Enterprises with appropriate support packages can enable the logs and receive the log events in near real time.
- The log events are surfaced through the APIs cloud logging and security command center.
- Record the action taken by Google personnel.
---
