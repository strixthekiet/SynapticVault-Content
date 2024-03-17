---
tags:
  - CompSci/cloud-computing/Terraform/Language
---
# Terraform Backend
### 1. Backend Config:
- Backends determine where [[CompSci/CloudComputing/Terraform/Terraform State|Terraform State]] is stored
	- must run [[terraform init]] to restart
	- `terraform init -migrate-state` to migrate where state is stored
- Stored as a backend block within `terraform` block
- Responsible for [[#6. Locking|State locking]]
	- not all backends support state locking
- Available backends:
	- Cant load additional backends as plugins
- Using **backend block**:
	- This tells Terraform where to store as backend
	- A config can only have 1 backend block
	- cant refer to named value
	- when using Terraform Cloud, it doesnt need to have backend block
### 2. Available backends:
- Local
	- 
	  ```hcl
		terraform {
		  backend "local" {
		    path = "terraform/state/terraform.tfstate"
		  }
		}
		```
- Remote
	- 
	  ```hcl
		  terraform {
			  backend "remote" {
				organization = "example_corp"
			
				workspaces {
				  name = "my-app-prod"
				}
			  }
			}
		```
- ...