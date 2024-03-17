---
tags:
  - CompSci/cloud-computing/GCP/product/Logging
---
# Logging Query Language
### Description:
- [Docs](https://cloud.google.com/logging/docs/view/logging-query-language)
- [All Log Fields](https://cloud.google.com/logging/docs/reference/v2/rest/v2/LogEntry)
- A recipe:
	- What do you know about the log entry?  
		- Log filename, resource, a bit of text?
	-  Full text searches are slow, but may be effective: 
		- "/score called" 
			- -> jsonPayload:”/score called”
			- or -> jsonPayload.message=”/score called”
		- or label
	-  Use indexed SEARCH function for complete text matches, because they perform a case-insensitive match
		- SEARCH(textPayload, "hello world")  
			- faster than global search
	-  If possible, restrict text searches to an log field
		-   jsonPayload:"/score called"
		-   jsonPayload.message="/score called"
# A. Overview:
- Using the `resource.type` field in the following examples, the Logging query language grammar looks like this:
	- Simple restriction: `resource.type = "gae_app"`
	- Conjunctive restriction: `resource.type = "gae_app" AND severity = "ERROR"`
	- Disjunctive restriction: `resource.type = "gae_app" OR resource.type = "gce_instance"`
	    - Alternatively: `resource.type = ("gae_app" OR "gce_instance")`
	- Complex conjunctive/disjunctive expression: `resource.type = "gae_app" AND (severity = "ERROR" OR "error")`
- Example:
	- `resource.type = "gce_instance" AND severity >= "ERROR" AND NOT textPayload:robot`
# B. Syntax notations:
### 1. Syntax summary:
- A query contains an expression
	- `expression = ["NOT"] comparison { ("AND" | "OR") ["NOT"] comparison }`
- A comparison is either a single value or a boolean expression:
	- `"The cat in the hat"`
		- global restriction
	- `resource.type = "gae_app`
### 2. Boolean operators:
- AND and OR and NOT:
	- `"a" OR NOT "b" AND NOT "c" OR "d"`
	- `("a" OR (NOT "b")) AND ((NOT "c") OR "d")`
- And and Or are short-circuit operators
- NOT has highest priority
	- can be replaced with `-`
### 3. Comparisons:
- `[FIELD_NAME] [OP] [VALUE]`
	- `[FIELD_NAME]` is path name of a a field in log entry
	- `[OP]` is comparison operator, is one of the following:
		- 
		  ```sql
			=           -- equal
			!=          -- not equal
			>< >= <=    -- numeric ordering
			:           -- "has" matches any substring
			:*          -- "has" any
			=~          -- regular expression search for a pattern
			!~          -- regular expression search not for a pattern
			```
	- `[VALUE]`: nb, string, function or expression or `NULL_VALUE`
 
### 4. Types of log fields:
### 5. Comments
### 6. Comparison operators:
### 7. Global restrictions:
### 8. Functions:
### 9. SEARCH function:
### 10. Using regular expressions:
- 
# C. Finding log entries quickly:
# D. 