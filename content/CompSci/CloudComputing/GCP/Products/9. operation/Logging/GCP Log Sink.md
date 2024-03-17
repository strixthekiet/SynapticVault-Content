---
tags:
  - CompSci/cloud-computing/GCP/product/Logging
---
# GCP Log Sink
### Description:
- An object created to hold a log query and routes to  a destination 
	- When GCP Logging service receives new log entries, they are compared against each sink (with the language) and decide where to store
	- with exclusion
- can be used to forward copies of some or all of log entires to non-default location
	- Logging bucket (default)
	- Bq
	- GS
	- Cloud Pub/sub topic
	- Splunk
	- GCP
	- Others, Splunk
### two