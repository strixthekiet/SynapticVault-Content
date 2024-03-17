---
tags:
  - CompSci/cloud-computing/Azure/service/Storage/file
---
# Azure Storage Sync
### 1. Overview:
- Sync many computers' drive to have the content of 1 [[Azure File Shares]]
- Using package Azure File Sync Agent:
	- has 3 components:
		- `FileSyncSvc.exe`: monitor changes on server endpoints
		- `StorageSync.sys`: supports cloud tiering
		- 
### 2. 
# A. Settings:
# B. Sync:
### 1. Azure Sync Group:
- A sync group defines the sync topology for a set of files. 
- Endpoints within a sync group are kept in sync with each other.
### 2. Registered Server:
- Represents a trust relationship between your server (or cluster) and the Storage Sync Service resource
---
### Server endpoint
### Cloud endpoint