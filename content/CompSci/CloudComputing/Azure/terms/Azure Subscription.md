---
tags:
  - CompSci/cloud-computing/Azure/term
---
# Azure Subscription
### Description:
- An Azure subscription links to an Azure account, which is an identity in Microsoft Entra ID or in a directory that Microsoft Entra ID trusts.
- Like a billing account
- Has a default subscription that links to the tenant of itself
- [[Azure Resource Group]] are organized into and billing is made
- Every Azure subscription can be associated with a Microsoft Entra ID. Users and services authenticate with Microsoft Entra ID before they access resources.
- There are two types of subscription boundaries that you can use:
	- **Billing boundary**: 
		- This subscription type determines how an Azure account is billed for using Azure. 
		- You can create multiple subscriptions for different types of billing requirements. Azure generates separate billing reports and invoices for each subscription so that you can organize and manage costs.
	- **Access control boundary**: Azure applies access-management policies at the subscription level, and you can create separate subscriptions to reflect different organizational structures. An example is that within a business, you have different departments to which you apply distinct Azure subscription policies. This billing model allows you to manage and control access to the resources that users provision with specific subscriptions.
### 