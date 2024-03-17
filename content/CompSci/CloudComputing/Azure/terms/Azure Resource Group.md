---
tags:
  - CompSci/cloud-computing/Azure/term
aliases:
  - resource group
---
# Azure Resource Group
### 1. Overview:
- Resource groups are simply groupings of [[Azure Resource]]
- can't be nested
- cannot be renamed
- can have resources from many different regions
- All the resources in your group should share the same lifecycle. You deploy, update, and delete them together. If one resource, such as a database server, needs to exist on a different deployment cycle it should be in another resource group.
- You can move a resource from one resource group to another group. Limitations do apply to [moving resources](https://learn.microsoft.com/en-us/azure/azure-resource-manager/management/move-support-resources).
- used to scope access control for administrative actions.
### 2. Activity logs:
- [[Azure Activity Log]]
### 3. Access Control
- [[Identity and Access Management|IAM]]
- [[Azure Role Based Access Control]]
### 4. Tags:
- Each resource tag consists of a name and a value. You could have the tag name `Server` and the value `Production` or `Development`, and then apply the tag/value pair to your Engineering computer resources.
- Tags applied to a resource group aren't inherited by the resources in the resource group.