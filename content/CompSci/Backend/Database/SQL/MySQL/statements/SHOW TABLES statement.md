---
mindmap-plugin: basic
tags:
  - CompSci/database/SQL/statement/db-administration
---
# SHOW TABLES statement
### Descriptions:
- Lists the non-`TEMPORARY` tables in a given database.
### Synopis:
- `SHOW`
	- `[EXTENDED]` 
	- `[FULL]`
	- `TABLES`
		- all the tables in the database
	- `[{FROM | IN} _db_name_]`
	- `[LIKE 'pattern' | WHERE expr]`
		- [[Like clause]] indicates which table names to match