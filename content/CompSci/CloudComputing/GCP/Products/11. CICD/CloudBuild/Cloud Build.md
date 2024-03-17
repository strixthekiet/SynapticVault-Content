---
tags:
  - CompSci/cloud-computing/GCP/product/CloudBuild
  - CompSci/dev/backend/container
aliases:
  - "#CompSci/cloud-computing/GCP/product/CloudBuild"
---
![|100](https://repository-images.githubusercontent.com/263972784/09732b80-9880-11ea-8f05-bad478ba140d)
# [Google Cloud Build](https://console.cloud.google.com/cloud-build)
### Description:
- Build [[Docker]]-compatible containers with either YALM or [[Dockerfile]]
	- `docker push gcr.io/`
	- `docker pulll gcr.io/`
- Save to artifact registry after built
- Can be configured to fetch dependencies, run unit test, static analysis and integration tests and create artifacts
- Automatically have integration testing
- `gcloud builds`
	- `gcloud builds submit . --tag gcp.io/project-name/img-name:v1`
	- needs img-name to not fail
### 4. Triggers:
- Can be ran in advance to test
- 
	- Region:
		- can be global
	- Tags:
		- trigger tag
- Event:
	- Repository event that invokes trigger
		- Push to a branch 
		- Push new tag 
		- Pull request 
			- Not available for Cloud Source Repositories
	- 
- Source:
	- Which repo [[Cloud Source Repositories]]
	- Which branch
- Configuration:
	- 



	- with branch name or by commit tag