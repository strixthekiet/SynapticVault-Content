---
tags:
  - CompSci/cloud-computing/GCP/product/ComputeEngine
  - CompSci/cloud-computing/GCP/product/CloudStorage
---
# Compute Engine Storage
### Description:
- Every Compute Engine VM instance is attached to at least one disk as a boot disk and for persistent storage. 
- A disk is partioned and managed by Google
### 1. Disks:
- Choose which [[Boot disk image]] for VM to start from
	- Custom or public
	- Some public images are premium, charged per second/minute
	- can be from [[#4. Compute Engine Machine image]]
	- So it will come with a single root persistent disk
- Advance
	- Deletion rule:
		- Normally the boot disk defaults to being deleted automatically when the instance is deleted. 
		- You can override it so u can ==recreate system [[Compute Engine Machine image]]== from boot disk of a terminated vm
- Persistent disk vs Local SSD vs RAM disk:
	- Persistent disk
		- Attached to the VM through the network interface, not physically
		- Survices if the Vm terminates
		- HDD vs SSD
		- Can be resized while its running
		- Can also attach a disk in read-only mode to multiple VMs.
			- Shared so cheaper than replica
		- Can be zonal or regional
			- pd-standard: persistence disk HDD
			- pd-ssd
			- ﻿﻿pd-balanced
			- ﻿﻿pd-extreme (zonal)
	- Local SSD:
		- Physically attached to the VM
		- Ephemeral but much faster than persistence
		- Lose data when Vm stop or terminate
		- Cant be shared between VMs
	- RAM disk:
		- tmpfs
		- fastest for high-memory vm
	- | | Persistent HDD | Persistent SSD | Local SSD | Ram disk
	  | --- | --- | --- | --- | --- |
	  | Data redundancy | Yes | Yes | No | No |
	  | Encryption at rest | Yes | Yes | Yes | N/A |
	  | Snapshotting | Yes | Yes | No | No |
	  | Bootable | Yes | Yes | No | Not |
	  | Use case | bulk file | faster | very fast | fastest but have data loss |
- Location:
- Source:
- 
- Location:
	- A disk can be in 1 regional but many zone as failover replica
- can have many disk with different os
- 
### 2. Snapshots
- Only available to persistent disk
- Are incremental, like git, unlike a machine image
- they can be used to:
	- backup critical data into a durable storage solution to meet application, availability, and recovery requirements.
	- Transfer data from 1 zone to another
	- transfer data to another disk type
- stored in [[Google Cloud Storage]]
### 3. [[Compute Engine Image]]