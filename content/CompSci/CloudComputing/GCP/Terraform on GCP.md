---
tags:
  - CompSci/cloud-computing/GCP
  - CompSci/cloud-computing/Terraform
---
# Terraform on GCP
### Description:
- [[Terraform]]
- [Docs](https://cloud.google.com/docs/terraform)
- [All modules](https://registry.terraform.io/providers/hashicorp/google/latest/docs)
- [Samples](https://github.com/orgs/terraform-google-modules/repositories)
### With GCP:
- provider.tf
	- `provider "google"{}`
- for a resource:
```
	  resource \[Resource_TYPE] "resource_name"{
		  name = [RESOURCE_NAME]
		  #Resouce properties
	  } 
```