---
tags:
  - CompSci/cloud-computing/GCP/product/ComputeEngine
  - CompSci/dev/backend
aliases:
  - GCE
  - Compute Engine
  - "#CompSci/cloud-computing/GCP/product/ComputeEngine"
---
![|100](https://media.datacenterdynamics.com/media/images/Google_Compute_Engine_logo2.width-358.png)
# Compute Engine
### Description:
- [[IaaS]]
- Has a default [[GCP Service Account|service account]]
- `gcloud compute`
- Move an instance to a new zone
	- ﻿﻿Automated process (moving within region):
		- ﻿﻿gcloud compute instances move
		- ﻿﻿Update references to VM; not automatic
	- ﻿﻿Manual process (moving between regions):
		- ﻿Snapshot all persistent disks on the source VM.
		- ﻿﻿Create new persistent disks in destination zone restored from snapshots.
		- ﻿﻿Create new VM in the destination zone and attach new persistent disks.
		- ﻿﻿Assign static IP to new VM.
		- ﻿﻿Update references to VM.
		- ﻿﻿Delete the snapshots, original disks, and original
- `gcloud compute config-ssh`
# A. [[GCP Virtual machines]]

# B. [[Compute Engine Storage]]

# C. [[Compute Engine Managed Instance Group]]


# D. VM manager:
- OS patch management???
	- patch compliance reporting
	- patch deployment
- You can select what patches to apply to your system from the full set of updates available for the specific operating system.
- You can set up flexible scheduling so you can choose when to run patches (one-time or recurring schedules).

# F. Settings:
### 3. [[GCP Network Endpoint Group]]
### 6. [[Compute Engine Setting]]

---