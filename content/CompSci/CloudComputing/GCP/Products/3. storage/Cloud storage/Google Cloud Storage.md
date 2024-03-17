---
tags:
  - CompSci/cloud-computing/GCP/product/CloudStorage
aliases:
  - gs
---
# [Google Cloud Storage](https://console.cloud.google.com/storage)
### Description:
- Offers developers and IT organizations durable and highly available [[Object storage|object storage]]
- For store anything in binary, such as image for Kubernetes,...
- Encrypt data on the server side
- Data travel between customer and Google by HTTPS/TLS
- Turn [[#Object versioning]] on to improve durability
- Upload through:
	- Online transfer (SDK, cloud console)
	- [[Storage Transfer]]
	- [[Transfer Appliance]]
	- Send usb/tape/... to facilities
- [[Blob]]:
	- Contains:
		- Binary
		- Relavant meta-data
		- Global unique identifier (in the form of URLs)
	- No minimum object size requirement
- Has links gs://sth
- `gcloud storage`
- `gsutil`
	- slower than gcloud storage
- Custom encrypt the file when send and receive in .boto file
###  1. [[Bucket]]s:
- All blobs are organized into buckets
	- Can be transfered from one to another bucket
- Buckets cant be nested
- Create bucket:
	- Name:
		- Buckets ID are **globally unique**
		- Labels
	- Where to store:
		- Multi region
		- Dual-region
		- Regional
	- ==Storage class==:
		- there is fee for store, different from retrieving
		- Bucket's class is applied to object classes, but changeable for individially
		- 
		- Classes
			- Autoclass:
				- Automatically transition to appropriate class based on the access pattern
			- Standard storage class: 
				- no retrieval cost.
				- no minimum storage duration
			- Nearline storage class:
				- For average once a month or less.
			- Coldline storage class:
				- For once every 90 days
			- Archive storage class:
				- Lowest cost, used for data archiving, backup, disaster recovery
				- For less than once a year
	- Controll access:
		- Uniform
		- Fine-grained ([[GCP Access Control List|ACL]])
	- 
- Objects
	- 
	- Maximum 100 entries
	- Signed URL
		- grants read or write access to a specific Cloud Storage resource and specifies when the access expires after an amount of time
- Configuration:
- ...
- Lifecycle
### 2. Monitoring

### Object versioning:
- Typically,  each new version to completely overwrite the older one
- Object versioning allows to keep track of each change made to a particular object by enabling “versioning” within a bucket.
	- like git versioning
	- Can restore, delete a version,...
	- Each version is 1 file
	- Can turnversioning off anytime:
		- leaves existing object versions in place, only replacing the newest version
		- causes the bucket to stop accumulating new archived object versions.
### Life-cycle management policies
- Based on a configuration, [[Google Cloud Storage|gs]] performs the specific action when 1 of the rule is met
	- Change to config can take up to 24 hours to have affects
	- Limiting the number of non-current versions per object and scheduling them to expire after a number of days
	- Retention policy: present deletion or modification of buckets's objects for a specific minimum duration of time after being uploaded
- life.json file with gsutil lifecycle set life.json `gs://$BUCKET_NAME_1`
### Customer-supplied encryption key (CSEK)
- gsutil and .boto file
### Directory synchronization:
- Synchronize the directory of a VM with the bucket
- 
### Object notification:
