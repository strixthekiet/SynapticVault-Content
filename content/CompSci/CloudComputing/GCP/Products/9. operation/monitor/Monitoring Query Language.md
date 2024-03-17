---
tags:
  - CompSci/cloud-computing/GCP/product/Monitoring/MQL
aliases:
  - MQL
---
# Monitoring Query Language, MQL
### Description:
- Expressive for quering time-series data
- Manipulate, retrive and perform operations
- Used to:
	- create ratio-based charts and alerts
	- Apply math, logic operations to metrics
	- Fetch, join, and aggregate over multiple metrics
	- Select by arbitrary, rather than predefined, percentile values
	- Create new labels to aggregate data by, using arbitrary string manipulations including regular expressions
- Built using operations and functions
- **Operations are linked by '|'** and **output of 1 op becomes input of the next op**
	- [[Pipe idiom]]
- [Docs](https://cloud.google.com/monitoring/mql/reference)
# Data Model
### Time series data:
- metrics: 
	- describes the metric
	- contains:
		- metric label: represents one combination of label values.
		- metric type: specifies the available labels and describes what is represented by the data points.
- resource:
	- records the resource label and specific monitored resource
	- represents one combination of lavel values and the specific monitored resource
	- resource-label
	- resource info
- metricKind and valueType:
	- metricKind:
		- gauge metric: measure an instant in time
		- delta metric: the change in time interval. request count 
		- cumulative metric: like bytes sent and received
	- valueType: data type, distribution is for an array
- points:
	- array of timestamped  values
### Tables
# Syntax and semantics
### Lexical elements
### Query structure:
- A query is made up of a sequence of table operations joined with a pipe operation `|`
# Table operations:
### Fetching:
- fetch:
	- Produces a table from the database
### Selection: