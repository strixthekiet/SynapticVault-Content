---
tags:
  - CompSci/cloud-computing/GCP/product/BigTable
  - CompSci/database/NoSQL
---
# Bigtable
### Description:
- Fully managed, wide-column [[NoSQL]] database that offers low latency and replication for high availability
	- Wide-column (key-value pairs with column families)
- Designed to handle massive workloads and big table with many columns
- Scale horizontal
- Great choice for both operational and analytical applications, including Internet of Things, user analytics, and financial data analysis.
- Choose Bigtable if:
	- working w >1tb of data
	- Data is fast with high thoughput or rapidly changing
	- Data is ==time-series== or has ==sematic ordering==
	- Running big data, asynchronous batch
	- ==Machine learning==
- Can interact with other services
	- ...
- Column family and column qualifier
	- Each row/column intersection can contain multiple cells, or versions, at different timestamps, providing a record of how the stored data has been altered over time.
- Cloud Bigtable tables are sparse; if a cell does not contain any data, it does not take up any space.
- A Cloud Bigtable table is sharded into blocks of contiguous rows, called tablets, to help balance the workload of queries.
- Similar to HBase api
- the smallest Cloud Bigtable cluster you can create has three nodes and can handle 30,000 operations per second.
- Remember that you pay for those nodes while they are operational, whether your application is using them or not.
### 