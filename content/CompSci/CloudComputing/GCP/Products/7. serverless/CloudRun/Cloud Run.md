---
tags:
  - CompSci/cloud-computing/GCP/product/CloudRun
  - CompSci/dev/backend/container
aliases:
  - "#CompSci/cloud-computing/GCP/product/CloudRun"
---
# [Cloud Run](https://console.cloud.google.com/run)
### Description:
- [[PaaS]]
- Managed compute platform that runs stateless containers via web requests or [[Cloud Pub-Sub]] events.
- Manage environment using containerized app
	- Serverless
	- Built on Knative
	- Automatically scale up and down extremely fast, charge only for the miliseconds it runs
- To deploy:
	1. Write the app
	2. Build and package to an container image
	3. Deploy to [[Artifact Registry]]
	- Or write the code and Cloud Run builds the image for you with Buildpacks
- Cloud Run then starts your container on demand to handle requests, and ensures that all incoming requests are handled by dynamically adding and removing containers.
- Can also run any binary, as long it is compiled for Linux 64 bits
- Needs a `app.yalm` file
- `gcloud run`
	- `gcloud app create --region=us-west1`
	- `gcloud auth configure-docker`
### 1. Services
- Create from existing image from
	- [[Artifact Registry]] or
	- [[Container Registry]] or
	- CICD from [[Cloud Source Repositories]]
- CPU allocation and pricing
- Autoscaling
- Authentication
- Containers
### 2. Jobs
### Manage custom domain:
- Can map custom domain to the cloud run url