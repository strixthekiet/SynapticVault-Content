---
tags:
  - CompSci/cloud-computing/Azure/service/AppService
---
# Azure App Service Plan
### Description:
- An app service always runs in an _App Service plan_.
- App Service plan associated with your Web Apps. Service plans determine the region used for the app datacenter, number of VMs used, and pricing tie
- `az appservice plan create --name $AZURE_APP_PLAN --resource-group $RESOURCE_GROUP --location $AZURE_REGION --sku FREE`
	- set to use free tier
- `az webapp create --name $AZURE_WEB_APP --resource-group $RESOURCE_GROUP --plan $AZURE_APP_PLAN`?
# A. Get
# C. Deployment and configuration:
- can be deployed from github