---
tags:
  - CompSci/cloud-computing/GCP/product/Security
aliases:
  - Identity-Aware Proxy
---
# Identity-Aware Proxy, GCP IAP
### Description:
- Lets you manage who has access to services hosted on App Engine, Compute Engine, or GCP Load Balancing
	- [[Private Google Access]]?
- Lets you establish a central authorization layer for applications accessed by HTTPS.
	- So you can use an application level access control model instead of relying on network level firewalls.
	- Applications and resources protected by Cloud IAP can only be accessed through the proxy by users and groups with the correct Cloud IAM role.
- Can be opened inside a GCP subnet
- [Using IAP for TCP forwarding  |  Identity-Aware Proxy  |  Google Cloud](https://cloud.google.com/iap/docs/using-tcp-forwarding)
- `gcloud compute ssh vm-internal --zone us-west1-c --tunnel-through-iap`
### 1. Applications
### 2. SSH and TCP Resources
### 3. Connectors