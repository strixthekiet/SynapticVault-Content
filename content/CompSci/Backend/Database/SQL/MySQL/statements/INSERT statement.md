---
mindmap-plugin: basic
tags:
  - CompSci/database/SQL/statement/data-manipulation
aliases:
  - INSERT
---
# INSERT statement
### Definition:
- Inserts new rows into an existing table. 
- The INSERT ... VALUES, INSERT ... VALUES ROW(), and INSERT ... SET forms of the statement insert rows based on explicitly specified values. 
- The INSERT ... SELECT form inserts rows selected from another table or tables. 
- You can also use INSERT ... TABLE in MySQL 8.0.19 and later to insert rows from a single table. 
- INSERT with an ON DUPLICATE KEY UPDATE clause enables existing rows to be updated if a row to be inserted would cause a duplicate value in a UNIQUE index or PRIMARY KEY. 
- In MySQL 8.0.19 and later, a row alias with one or more optional column aliases can be used with ON DUPLICATE KEY UPDATE to refer to the row to be inserted.
### INSERT
- INSERT 
	- 

### Referrences:
- _value_: 
	- {_expr_ | DEFAULT}
- _value_list_:
	- _value_ [, _value_] ... 
- _row_constructor_list_: 
	- ROW(_value_list_)[, ROW(_value_list_)][, ...] 
- _assignment_: 
	- _col_name_ = 
		- _value_ 
		- | [_row_alias_.]_col_name_
		- | [_tbl_name_.]_col_name_ 
		- | [_row_alias_.]_col_alias_ 
- _assignment_list_: 
	- _assignment_ [, _assignment_] ...


