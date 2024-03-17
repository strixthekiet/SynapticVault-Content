---
mindmap-plugin: basic
tags:
  - CompSci/database/NoSQL
  - CompSci/cloud-computing/GCP/product/Firestore
aliases:
  - "#CompSci/cloud-computing/GCP/product/Firestore"
---
# Firestore
### Description:
- Flexible, ==horizontally scalable==, [[NoSQL]] cloud database for mobile, web, and server development.
	- automatic multi-region data replication
	- strong consistency guarantees
	- atomic batch operations
	- real transaction support.
- Unit max size 1mb
- Schedule export job for better durability
- Data is stored in documents then organized into collections of documents
	- Like a Json file
	- 📚 users
		- 📗 alovelace  
			  first : "Ada"  
			  last : "Lovelace"  
			  born : 1815  
		- 📗 sride  
			  first : "Sally"  
			  last : "Ride"  
			  born : 1951  
	- 📚 rooms
		- 📗 software
			- 📚 messages
				- 📗 message1  
					  from : "alovelace"  
					  content : "..."  
				- 📗 message2  
					  from : "sride"  
					  content : "..."
- Billing charged for each document read, write, and delete that you perform with Firestore.
	- Has 50k reads, 20k write, 20k deletes, 1gb of data for free per day
- The db reference caches data that an app is actively using, so the app can write, read, listen to, and query data even if the device is offline.
	- When the device comes back online, Firestore synchronizes any local changes back to Firestore. 
- Automatic multi region replication
- Pays per read/write
### Native mode vs Datastore mode
- Next gen of [[GCP Datastore]]
- Datastore
	- real time updates in mobile and web client library features are not.
	- For server project
- Native:
	- compatitble with all datatore
	- Firestore can operate in datastore mode, so its backward compatible
### ACID transaction?
- 
