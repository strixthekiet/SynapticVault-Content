---
mindmap-plugin: basic
tags:
  - CompSci/cloud-computing/GCP/product/shell
aliases:
  - Cloud Shell
---
![|100](https://img.stackshare.io/service/25414/default_d809010e0ae609bdef4a7949425d39ff5bffe573.png)
# Google Cloud Shell
### Description:
- https://cloud.google.com/sdk/gcloud/reference
- Each of the `gcloud GROUP` is used different for each of the service, from each of the group
	- Also have ==gsutil== and ==bq==
- At all points, use help `gcloud help <group>`
	- then use `/` to search
	- or man
- Use `gcloud alpha interactive`
- `gcloud auth`
	- `gcloud auth login`
	- `gcloud auth application-default login` to authenticate the shell
- `gcloud config`
	- `gcloud config set project <projec_id>`
### Cloud shell:
- Has [[Terraform]] built in
- You can upload a file and download from the vm instance
- A temporary Compute Engine VM which is a part of Cloud VPC network
	- Command-line access to the instance via a browser
	- logged in by project's default service account
- 5 GB of persistent disk storage ($HOME dir)
	- After 1 hour of inactivity, the Cloud Shell instance is recycled. 
	- Only the /home directory persists. 
	- Any changes made to the system configuration, including environment variables, are lost between sessions.
- Pre-installed Cloud SDK and other tools
	- gcloud: for working with Compute Engine and many Google Cloud services
	- gcloud storage: for working with Cloud Storage
	- kubectl: for working with Google Kubernetes Engine and Kubernetes
	- bq: for working with BigQuery
	- Language support for Java, Go, Python, Node.js, PHP, and Ruby
- Web preview functionality
- Built-in authorization for access to resources and instances

### Modify the bash profile and create persistence
- Create persistence variable names in CLI?
### Commonly used
- Quick start: `gcloud cheat-sheet`