---
tags:
  - CompSci/cloud-computing/GCP/product/CloudCDN
  - CompSci/network/server
---
# Cloud CDN
### Description:
- Has global system of [[Edge caching|edge caches]]
- Lower latency, less load in 1
- Enable in a check box
- Cache hit vs cache miss
- Automatically logged within Google Cloud.
- cache modes control what to be cached
	- define how responses are cached, whether or not Cloud CDN respects cache directives sent by the origin, and how cache TTLs are applied.
	- 3 modes:
		- USE_ORIGIN_HEADERS mode requires origin responses to set valid cache directives and valid caching headers.
		- CACHE_ALL_STATIC mode automatically caches static content that doesn't have the no-store, private, or no-cache directive.
			- Origin responses that set valid caching directives are also cached.
		- FORCE_CACHE_ALL mode unconditionally caches responses, overriding any cache directives set by the origin.
		- 