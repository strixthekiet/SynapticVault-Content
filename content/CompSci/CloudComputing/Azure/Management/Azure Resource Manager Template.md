---
tags:
  - CompSci/cloud-computing/Azure/service/ResourceManager
aliases:
  - ARM template
---
# Azure Resource Manager Template
### Description:
- Defines all [[Azure Resource|resources]] and its dependencies in 1 deployment
	- can deploy into a [[Azure Resource Group|resource group]]
- Can also use parameters
### Syntax:
- [Doc](https://learn.microsoft.com/en-us/azure/azure-resource-manager/templates/syntax)
- Use with Azure ARM tools extension on VScode
	- Other editors (including Visual Studio) may not be able to process this schema. For those editors, use: [this](https://schema.management.azure.com/schemas/2015-01-01/deploymentTemplate.json#) 
	- For subscription deployments, use: [this](https://schema.management.azure.com/schemas/2018-05-01/subscriptionDeploymentTemplate.json#) 
	- For management group deployments, use: [this](https://schema.management.azure.com/schemas/2019-08-01/managementGroupDeploymentTemplate.json#) 
	- For tenant deployments, use: [this](https://schema.management.azure.com/schemas/2019-08-01/tenantDeploymentTemplate.json#)

| Element            | Description                                                                                                                                                                                                                                                                                                                              |
| ------------------ | ---------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------- |
| **schema**         | A required section that defines the location of the JSON schema file that describes the structure of JSON data. The version number you use depends on the scope of the deployment and your JSON editor.                                                                                                                                  |
| **contentVersion** | A required section that defines the version of your template (such as 1.0.0.0). You can use this value to document significant changes in your template to ensure you're deploying the right template.                                                                                                                                   |
| **apiProfile**     | An optional section that defines a collection of API versions for resource types. You can use this value to avoid having to specify API versions for each resource in the template.                                                                                                                                                      |
| **parameters**     | An optional section where you define values that are provided during deployment. These values can be provided by a parameter file, by command-line parameters, or in the Azure portal.                                                                                                                                                   |
| **variables**      | An optional section where you define values that are used to simplify template language expressions.                                                                                                                                                                                                                                     |
| **functions**      | An optional section where you can define [user-defined functions](https://learn.microsoft.com/en-us/azure/azure-resource-manager/templates/template-user-defined-functions) that are available within the template. User-defined functions can simplify your template when complicated expressions are used repeatedly in your template. |
| **resources**      | A required section that defines the actual items you want to deploy or update in a resource group or a subscription.                                                                                                                                                                                                                     |
| **output**         | An optional section where you specify the values that will be returned at the end of the deployment.                                                                                                                                                                                                                                     |