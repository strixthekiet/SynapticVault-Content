---
mindmap-plugin: basic
tags:
  - CompSci/database/SQL/statement/data-manipulation
---
# DESCRIBE statement
### Definition:
- Provides information about the columns in a table:
### DESCRIBE
- {EXPLAIN | DESCRIBE | DESC}
	- tbl_name 
	- [col_name | wild]
- {EXPLAIN | DESCRIBE | DESC}
	- [explain_type] 
	- [INTO variable]
	- {[schema_spec] explainable_stmt | FOR CONNECTION connection_id}
- {EXPLAIN | DESCRIBE | DESC} 
	- ANALYZE 
	- [FORMAT = TREE] 
	- [schema_spec] 
	- select_statement
### References
- explain_type:
	- FORMAT = format_name
- format_name:
	- TRADITIONAL
	- | JSON
	- | TREE
- explainable_stmt: 
	- [[SELECT statement]]
	- | [[TABLE statement]]
	- | [[DELETE statement]]
	- | [[INSERT statement]]
	- | [[REPLACE statement]]
	- | [[UPDATE statement]]
- schema_spec:
	- FOR {SCHEMA | DATABASE} schema_name
