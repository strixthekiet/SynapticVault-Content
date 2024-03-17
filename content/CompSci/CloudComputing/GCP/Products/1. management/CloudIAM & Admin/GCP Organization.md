---
tags:
  - CompSci/cloud-computing/GCP/product/CloudIAM
---
# GCP Organization
### Description:
- Root node in the GCP resource hierarchy.
- Can have sub-organization
- Organization roles:
	- ﻿﻿Organization Admin: Control over all cloud resources; useful for auditing
	- ﻿﻿Project Creator: Controls project creation, control over who can create projects
- Associated with G-Suite or ==Cloud Identity account==
### Workspace or Cloud identity super administrator:
- ﻿﻿Assign the Organization admin role to some users
- ﻿﻿Be the point of contact in case of recovery issues
- ﻿﻿Control the lifecycle of the Workspace or Cloud Identity account and Organization resource
### Organization admin:
- Defines IAM policies
- Determine the structure of resource hierachy
- Delegate responsibility over critical components such as Networking, Billing, and Resource Hierarchy through IAM roles
### Admin vs view role:
---