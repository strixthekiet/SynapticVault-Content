---
tags:
  - CompSci/cloud-computing/GCP/product/CloudStorage
aliases:
  - ACL
---
# GCP Access Control List, ACL
### Description:
- A mechanism you can use to define who has access to your buckets and objects, as well as what level of access they have.
- More fine-grained than IAM & Admin, rather than inherit from project to bucket to object
- In gs, you apply ACLs to individual buckets and objects.
	- https://cloud.google.com/storage/docs/access-control/lists
	- https://console.cloud.google.com/storage/create-bucket
- Include:
	- scope (user or group of user) 
		- 
	- permission (what can be performed on)