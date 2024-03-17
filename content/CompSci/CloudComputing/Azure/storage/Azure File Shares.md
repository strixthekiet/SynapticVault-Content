---
tags:
  - CompSci/cloud-computing/Azure/service/Storage/file
---
# Azure File Shares
### Description:
- Managed file shares for cloud or on-premises deployments.
- Native directory
- Azure Files enables you to set up highly available network file shares. Shares can be accessed by using the Server Message Block (SMB) protocol and the Network File System (NFS) protocol. 
	- Multiple [[Azure Virtual Machine]] can share the same files with both read and write access. 
	- You can also read the files by using the REST interface or the storage client libraries.
# Operations
### 1. Snapshots:
- Provided at file share level
- Incremental meaning only change are updated
- If want to delete a share that has share snapshots, first delete all its snapshot
### 2. Backup