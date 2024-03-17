---
tags:
  - CompSci/cloud-computing/GCP/product/Monitoring
---
![|100](https://static-00.iconduck.com/assets.00/cloud-monitoring-icon-2048x1385-zfw4etf9.png)
# Cloud Monitoring
### Description:
- Dynamically configures monitoring after resources are deployed and has intelligent defaults that allow you to easily create charts for basic monitoring activities.
- A metrics scope is the root entity that holds monitoring and configuration information in Cloud Monitoring.
	- belongs to  a [[GCP Scoping Project|Scoping project]]
	- Each metrics scope can have between 1 and 100 monitored projects.
	- 1 [[GCP project]] can only be monitored by 1 metric scope
	- `monitoring.viewer`
	- Only monitoring relies on Metric scope, all other resources belongs to project
- Can be from other common applications components, apache,...
- A lot of metrics are for free
- Can also monitor hybrid cloud with Bindplane
- Uses [[Monitoring Query Language|MQL]]
- Group:
	- Monitor a set of resources together as a single group. 
	- Groups can then be linked to alerting policies, dashboards, etc. 
	- Each metrics scope can support up to five-hundred groups and up to six layers of sub-groups. 
	- Groups can be created using a variety of criteria, including labels, regions, and applications.
### Cloud Monitoring agent:
- A collected-based daemon that gathers system and application metrics from virtual machine instances and sends them to Monitoring. 
- By default, the Monitoring agent collects disk, CPU, network, and process metrics. 
- Configuring the Monitoring agent allows third-party applications to get the full list of agent metrics.
### 1. Overview
- 
### 2. Dashboard
- Create dashboard with many tools to monitor resources
- Use this, so cool
### 3. 
### 4. Services:
- Consolidated services overview page is your point of entry.
- Define [[Service Level Objective|SLO]] directly, easily and let it monitor
	- Request-based SLO:
		- good request/total requests
	- Window-based SLO:
		- total nb of good/ bad requests
- Can create [[GCP Alert Policy|alert]] with SLO too
### 5. Metric explorer:
- For analyzing 1 type of any metric only, rather than many like a dashboard
- Then create a chart and :
	- share a link for use 
	- use it in [[#2. Dashboard]]
- Can use:
	- filter
	- aggregation
		- specifies how to display when there are multiple lines
	- sort and limit
	- min interval
- Analysis mode:
	- Standard mode displays each time series with a unique color.
	- Stats mode displays common statistical measures for the data in a chart.
	- X-ray mode displays each time series with a translucent gray color.
		- Each line is faint where lines overlap or cross the point appear brighter.
		- More useful for charts with many lines.
### 7. [[GCP Alert Policy]]
### 8. Uptime check:
- Send request to service every bit of time to check
	- can be set to HTTP(s) or TCP
- Set alert when it cant reach or the server is down
- Can check:
	- App Engine application
	- A Compute Engine instance,
	- A URL of a host, or
	- An AWS instance
	- A load balancer
### 10. Groups:
- Monitoring lets you define and monitor groups of resources, such as VM instances, databases, and load balancers. 
	- Based on names, type, tags, label
- You can organize resources into groups based on criteria that make sense for your applications.
- And subgroup