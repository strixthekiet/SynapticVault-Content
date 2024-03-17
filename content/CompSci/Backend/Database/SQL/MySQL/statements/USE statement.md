---
mindmap-plugin: basic
tags:
  - CompSci/database/SQL/statement/data-manipulation
aliases:
  - USE
---

# USE
### Definition:
- Tells MySQL to use the named database as the default (current) database for subsequent statements. This statement requires some privilege for the database or some object within it.
- The named database remains the default until the end of the session or another `USE` statement is issued
- The database name must be specified on a single line. Newlines in database names are not supported.
- Making a particular database the default by means of the USE statement does not preclude accessing tables in other databases. The following example accesses the `author`table from the `db1` database and the `editor` table from the `db2` database:
	- ```sql
	  USE db1; SELECT author_name,editor_name FROM author,db2.editor WHERE author.editor_id = db2.editor.editor_id;```
### USE
1. _db_name_
