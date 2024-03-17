---
tags:
  - CompSci/cloud-computing/Terraform/Language
aliases:
  - Terraform State
---
# Terraform State
### 1. 
- Snapshot of infrastructure
- 
- In file the default file `terraform.tfstate`
	- json format
- Can be stored in **Terraform Cloud**
- Inspection and Modification
	- Shouldnt be modified
	- state remove, forget?
- Format:
	- can use with `terraform output -json`
	- can use with `terraform show -json`
### 2. Purpose:
- To map real world resources
	- To guarantee one-to-one mapping
- To track of metadata:
	- like dependencies
- For `terraform plan` to work faster
- For sharing
- **State locking**?
- Workspace:
	- Terraform backend?
### 3. The terraform_remote_state data source:
- x
### 4. Terraform Backend
### 5. Import existing resources:
### 6. State Locking:
- If supported by backend, Terraform will lock states for all operations that could write state
	- happens automatically on all operations that could write state
- [[terraform force-unlock]]