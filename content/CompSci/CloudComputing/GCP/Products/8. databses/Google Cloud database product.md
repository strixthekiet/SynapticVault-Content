---
mindmap-plugin: basic
tags:
  - CompSci/database
  - CompSci/cloud-computing/GCP/product
---
# Google Cloud database product
### Description:
- 
### Decision tree:
- Is ur data structured?:
	- Yes -> Does it need analytics?
		- Yes -> Do you need extensive update and/or low latency?
			- Yes -> [[Bigtable]]
			- No -> [[BigQuery]]
		- No -> Is ur data relational?
			- Yes -> Do you need [[HTAP]]?
				- Yes -> [[AlloyDB]]
				- No -> Do you need global scalability?
					- Yes -> [[Cloud Spanner]]
					- No -> [[Cloud SQL]]
			- No -> Need application caching?
				- Yes -> [[GCP Memorystore]]
				- No -> [[Firestore]]
	- No -> Need a shared file system?
		- Yes -> [[Filestore]]
		- No -> [[Google Cloud Storage]]
- [[GCP Database Migration]]
### Storage configuration:?
- Archive: use less than once a year
- Coldline: use less than once per 90 days
- Nearline: less than once a month
- Standard