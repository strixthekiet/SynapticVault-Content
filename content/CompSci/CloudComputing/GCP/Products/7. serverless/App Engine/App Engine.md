---
tags:
  - CompSci/cloud-computing/GCP/product/AppEngine
aliases:
  - "#CompSci/cloud-computing/GCP/product/AppEngine"
---
![|100](https://w7.pngwing.com/pngs/114/539/png-transparent-google-app-engine-google-cloud-platform-google-compute-engine-cloud-computing-engine-blue-trademark-logo.png)
# [App Engine](https://console.cloud.google.com/appengine)
### Description:
- [[PaaS]]
- [Use this](https://github.com/GoogleCloudPlatform/training-data-analyst/tree/master/courses/design-process/deploying-apps-to-gcp)
- Automatic load balancing
- Just write the code, no need to worry about hardware
- App engine **Flexible** supports **custom container**
- Batch app
- mem cache? cache queries
- Cloud task?
	- perform work asyn outside user request
- `gcloud app`
	- `gcloud app create`
	- `gcloud app deploy`

| Feature | Standard Environment | Flexible Environment |
| ---- | ---- | ---- |
| Managed | Yes | No |
| Languages | Python, Java, Node.js, PHP, Ruby, Go | Any |
| Scaling | Automatic | Manual |
| Built-in services | Yes | No |
| Pay-per-use | Yes | No |
| Security restrictions | More | Less |
| Control | Less | More |
| Cost | Lower for bursty workloads | Higher |
| Custom image | No | Yes |
### 1. Dashboard:
- 1 project has 1 App Engine app
- 1 app has 1 or more [[#2. Services|services]]
### 2. Services:
- 1 service has 1 or more [[#3. Versions|versions]]
### 3. Versions:
- 1 version has 1 or more [[#4. Instances|instances]]
- Can have multiple version and split traffic between them
	- tag `--no-promote`
### 4. Instances:
- [[GCP Virtual machines]]