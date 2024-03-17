---
tags:
  - CompSci/cloud-computing/Terraform/CLI
---
# terraform plan
### Description:
- Creates an execution plan
	- lets you preview the changes that Terraform plans to make to your infrastructure. 
- By default, when Terraform creates a plan it:
	- Reads the current state of any already-existing remote objects to make sure that the Terraform state is up-to-date.
	- Compares the current configuration to the prior state and noting any differences.
	- Proposes a set of change actions that should, if applied, make the remote objects match the configuration.
- Does not actually carry out the proposed changes 
	- use this command to check whether the proposed changes match what you expected
- 
### Synopsis:
