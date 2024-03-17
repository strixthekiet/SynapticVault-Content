---
tags:
  - CompSci/cloud-computing/GCP/product/Monitoring/Alert
---
# GCP Alert Policy
### Description:
- Has:
	- A name
	- ﻿﻿One or more conditions
	- ﻿﻿Notifications
	- ﻿﻿Documentation
- In YAML or Json format
- https://cloud.google.com/sdk/gcloud/reference/alpha/monitoring/channels/create
- Can monitoring in a group with multiple resources
- Design alert:
	- If too short window: easier for false positive
	- If too long window: less false positive byt longer to detect fail of SLOs and takes more of error budget
	- Set alert of short windows with successive failture counts
### Types of alert policies:
| Metric-based alerting policies | [[Cloud Logging#4. Log-based metrics\|Log-based]] alerting policies |
| ---- | ---- |
| for metric data collected by Cloud Monitoring | for a specific message occured in the Log |
| Add in Alert of Cloud Monitoring | Add in Log Explorer or Alert of Monitoring |
|  |  |
- Metric-based alerts:
	- types of conditions:
		- Metric threshold: more than or equal a threshold
		- Metric absence: when there is absence of a metric measurement
		- Forecase: predicts
### Alert condition:
- Decide what's being monitored and under what condition an alert must be generated.
- 