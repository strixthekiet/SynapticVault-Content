---
tags:
  - CompSci/cloud-computing/Azure/service/Storage
author: container
---
# Azure Storage Container
### Description:
- Azure's version of a [[Bucket]]
- A group of Azure's [[Azure Blob]]
- Must be unique within the storage account
- Public access level: 
	- The access level specifies whether the container and its blobs can be accessed publicly. 
	- By default, container data is private and visible only to the account owner. 
	- There are three access level choices: 
		- Private: (Default) Prohibit anonymous access to the container and blobs. 
		- Blob: Allow anonymous public read access for the blobs only. 
		- Container: Allow anonymous public read and list access to the entire container, including the blobs.
			- only if anonymous access has been allowed for the storage account.
			- Anonymous access is controlled at the container level, not for individual blobs. 
			- So, if you want to secure some of the files, you need to put them in a separate container that doesn't permit public read access.
### As Data Lake:
- can be a data lake whe enabled **hierarchical--namespace**
