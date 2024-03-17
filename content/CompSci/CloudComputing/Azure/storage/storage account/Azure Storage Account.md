---
tags:
  - CompSci/cloud-computing/Azure/service/Storage
---
# Azure Storage Account
### Descriptions:
- [Configure](https://www.youtube.com/watch?v=AhuNgBafmUo)
- All storage account types are encrypted at rest by Storage Service Encryption
- Configure the storage account to allow public access by setting the _AllowBlobPublicAccess_ property. 
	- When set to true, Blob data is available for public access only if the container's public access setting is also set.
### 1.  Overview:
- Essentials:
	- Belongs to a [[Azure Resource Group|resource group]] in a [[Azure Region]]
	- 
- Properties:
- Monitoring:
- Capabilities:
- .
- Tools + SDKs:
	- Python SDK and cli

### 2. Activity log
### 3. [[Azure Tag|Tag]]
### 4. Diagnose and Solve Problems:
### 5. IAM
### 6. Data Migration:
- Use `Az-Copy` PS or `azcopy` in CLI
- Or [[Azure Data Box]]
### 7.
### 8. Storage Browser:
# A. Data storage:
### 1. [[Azure Storage Container]]
- ![](https://learn.microsoft.com/en-us/azure/storage/blobs/media/storage-blobs-introduction/blob1.png)
- 
### 2. [[Azure File Shares]]
### 3. Queues:
- A messaging store for reliable messaging between application components.
- Queue messages can be up to 64 KB in size, and a queue can contain millions of messages. Queues are used to store lists of messages to be processed asynchronously.
### 4. Tables:
- A service that stores nonrelational structured data (also known as structured NoSQL data).
# B. Security + Networking:

### 1. Networking:
- Fire wall and virtual network
	- 
- Private Endpoint Connection:
	- using [[Azure Private Link]]
- Custom domain: ^863240
	- Doent currently provide native support for HTTPS with custom domains. 
		- You can implement an Azure Content Delivery Network (CDN) to access blobs by using custom domains over HTTPS.
	- 2 ways of configure custom domain:
		- Direct mapping:
			- Use [[#5. Endpoints|endpoint]] as CNAME in custom domain
		- Intermediary domain mapping:
			- Applies to a domain that is already in Azure
			- By prepending the asverify keyword to your own subdomain, you permit Azure to recognize your custom domain without modifying the DNS record for the domain. 
			- After you modify the DNS record for the domain, your domain is mapped to the blob endpoint with no downtime. 
			- example: 
				- CNAME record: `asverify.blobs.contoso.com `
				- Intermediate CNAME record: `asverify.contosoblobs.blob.core.windows.net`
### 2.
### 3.
### 4. [[Azure Shared Access Signature]]
### 5. Encryption:
- Manage encryption by using Microsoft's key or Customer's key
	- Customer's key can be from [[Azure Key Vault]]

# C. Data Mangement:
### 1. Storage task:
### 2. Redundancy:
- Replication strategies:
	- Locally Redundant Storage (LRS):
		- 3 disks in the same zone
	- Zone Redundant Storage (ZRS):
		- Synchrinously replicate data over 3 zones in a region
	- Geo-redundant Storage (GRS):
		- 16 9s durability
		- Replicate across 1 more region
		- RA-GRS is based on GRS
	- Geo-zone-redundant Storage (GZRS):
		- Replicate across 1 secondary region and also 3 zones in primary region
### 3. Data protection:
- Recovery
- Tracking:
	- Enable [[Azure Blob]] Versioning
	- [[Azure Blob]] change feed
- Access Control:
	- 
### 4. Object replication:
- Using [[Azure Replication Policy]], asynchronously replicate blob containers between containers of different Storage Account
- Required blob versioning is enabled on both source and destination
- Doesnt support blob snapshot
- Support for hot, cool, cold
	- source and destination account can be in different tiers
- 
### 7. Lifecycle Management:
- Can add a rule to delete or to change [[#^8a63cd|blob access tiers]] to another
# D. Settings:
### 1. Configuration:
- **Account Kind:**
	- **StorageV2 (general purpose v2)**:
		- Uses HDD
		- Support Blob, queue, table and files
	- **Premium block blobs**:
		- Uses SSH
		- Blob Storage (including Data Lake Storage)
		- Premium storage account for [[Azure Block Blob]] and [[Azure Append Blob]].
			- Recommended for applications with high transaction rates.
	- **Premium file shares**
		- For file shares only. 
		- Recommended for enterprise or high-performance scale applications. 
		- Use Premium file shares if you require support for both Server Message Block (SMB) and NFS file share
	- **Premium page blob**:
		- For [[Azure Page Blob]] only. Page blobs are ideal for storing index-based and sparse data structures, such as operating systems, data disks for virtual machines, and databases.
- Performance tier:
	- Standard storage accounts are backed by magnetic drives and provide the lowest cost per GB. They're best for applications that require bulk storage or where data is accessed infrequently. 
	- Premium storage accounts are backed by solid state drives and offer consistent, low-latency performance. They can also be used with Azure virtual machine disks, and are best for I/O-intensive applications, like databases.
- Secure transfer required:
	- s
- s
- Blob access tier (default):
	- Set the default access tier for a blob
	- Blob access tiers:  ^8a63cd
		- **Hot**
		- **Cool**
		- **Cold**
		- **Archive**
	- Each blob can have their own tier
### 2. Data Lake Gen2 Update:
### 3. Resource Sharing (CORS):
- Allow the storage account to be accessed from another site
### 4. 
### 5. Endpoints:
- Each service has their end point and follow by the specific object
- In the form `https://<storage-account>.<service>.core.windows.net/../..`
	- ex: `https://storageaccount.blob.core.windows.net/container/blob1`
- Can have [[#^863240|custom domain]] to mask the long URL
# E. Monitoring:
### 