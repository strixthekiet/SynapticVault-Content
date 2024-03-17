---
mindmap-plugin: basic
tags:
  - CompSci/cloud-computing/GCP/term
aliases:
  - service account
---
# GCP Service Account
### Description:
- Account for an application or compute workload instead of an individual end user.
- Can treat the service account as a resource and decide ==who can use it== by provisioning users or a group with the ==Service Account User== role.
	- For the role, manage permission
- All projects come with a Google Cloud APIs service account
	- identifiable by the email project-number@cloudservices.gserviceaccount.com.
- Represents a service
	- ex: firebase-adminsdk-owtll@lightseeker-chatbot.iam.gserviceaccount.com
- The service account runs the code for you as a product, so the billing can be counted
- Types of service accounts:
	-  ==Custom==
		- Use this
	- ﻿﻿Built-in
		- ﻿﻿Compute Engine and App Engine default service accounts
	- ﻿Google APIs service account
		- ﻿﻿Runs internal Google processes on your behalf (like firebase)
- Managed by:
	- Google-managed:
		- Google stores both the public and private portion of the key.
		- ﻿﻿Each public key can be used for signing for a maximum of two weeks.
		- ﻿﻿Private keys are never directly accessible.
	- User-managed service accounts
		- Google only stores the public portion of a user-managed key.
		- ﻿﻿Users are responsible for private key security.
		- ﻿﻿Can create up to 10 user-managed service account keys per service.  
		- Can be administered via the IAM API, gcloud, or the console.
### Permissions
### Keys
- You can create keys that can act as the service account then other project/user can use it with only specified actions
	- as json file
- `gcloud iam service-accounts keys create /tmp/key.json --iam-account service-account-name@${GOOGLE_CLOUD_PROJECT}.iam.gserviceaccount.com`
- `gcloud auth activate-service-account  --key-file=/tmp/key.json`