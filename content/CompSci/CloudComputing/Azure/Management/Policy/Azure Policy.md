---
tags:
  - CompSci/cloud-computing/Azure/service/Policy
---
# Azure Policy
### Description:
- Defines the how the resources are created and configured
- One or more policy definitions are grouped into an [[Azure Initiative Definition]], to control the scope of your policies and evaluate the compliance of your resources.
### Consider:
- **Consider deployable resources**. Specify the resource types that your organization can deploy by using Azure Policy. You can specify the set of virtual machine SKUs that your organization can deploy.
- **Consider location restrictions**. Restrict the locations your users can specify when deploying resources. You can choose the geographic locations or regions that are available to your organization.
- **Consider rules enforcement**. Enforce compliance rules and configuration options to help manage your resources and user options. You can enforce a required tag on resources and define the allowed values.
- **Consider inventory audits**. Use Azure Policy with Azure Backup service on your VMs and run inventory audits.
# B. Authoring:
### 1. Definitions:
- [List of built-in policy definitions](https://learn.microsoft.com/en-us/azure/governance/policy/samples/built-in-policies)
### 2. Assignments:
- A _policy definition_ describes the compliance conditions for a resource, and the actions to complete when the conditions are met.
- 
