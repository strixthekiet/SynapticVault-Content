---
tags:
  - CompSci/cloud-computing/Azure/service/RBAC
aliases:
  - RBAC
---
# Azure Role Based Access Control
### A. Overview:
- RBAC lets you determine what operations specific users can do on specific resources, and control what areas of a resource each user can access.
- Authorization system built on Azure Resource Manager. Azure RBAC provides fine-grained access management of resources in Azure.
- The system subtracts _NotActions_ permissions from _Actions_ permissions to determine the _effective permissions_ for a role.
# D. Concepts:
### 1. Role definitions:
- ![](https://learn.microsoft.com/en-us/azure/role-based-access-control/media/shared/rbac-role-definition.png)
- Different from Entra role
- Actions format:
	- `{Company}.{ProviderName}/{resourceType}/{action}`
	- can be:
		- `*`
		- `read`
		- `write`
		- `action`
		- `delete`
- Actions:
	- The `Actions` permission specifies the control plane actions that the role allows to be performed. It is a collection of strings that identify securable actions of Azure resource providers. Here are some examples of control plane actions that can be used in `Actions`.
	- `*/read`: read actions for all resources
	- `Microsoft.Compute/*`: All actions types on Microsoft.Compute provider
	- `Microsoft.Network/*/read`
	- `Microsoft.Compute/virtualMachines/*`
	- `microsoft.web/sites/restart/Action`
### 2. Role Assignment:
- An **assignment** attaches a [[#1. Role definitions|role definition]] to a **[[Azure Security Principal]]** at a particular **scope**. 
	- Users can grant the access described in a role definition by creating (attaching) an assignment for the role.
- Assign the _User Access Administrator_ role to an admin group scoped to a management group 
- Assign the _Contributor_ role to a user scoped to a subscription
### 3. Scope:
- The boundary for the requested _level_ of access, or "how much" access is granted.
- Management group, subscription, resource group, resource
### 4. 
---