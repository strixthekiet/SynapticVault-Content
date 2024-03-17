---
tags:
  - CompSci/cloud-computing/GCP/product/ComputeEngine
---
# Compute Engine Setting
### Description:
- 
	- sad
### 1. Metadata:
- Every VM instance stores its metadata on a metadata server.
- Compute Engine metadata lets you specify key-value pairs that are available to all VM instances in the project. 
	- A VM instance can query metadata as needed or it can wait to be notified of changes.
- Because the default metadata keys are the same on every instance, you can reuse your script without having to update it for each instance
	- this helps you create less brittle code for your applications.
### 2. Zones:
