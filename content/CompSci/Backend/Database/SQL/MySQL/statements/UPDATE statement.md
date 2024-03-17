---
mindmap-plugin: basic
tags:
  - CompSci/database/SQL/statement/data-manipulation
---
# UPDATE statement
### Definition:
-s
### UPDATE
1. [LOW_PRIORITY] 
2. [IGNORE] 
3. _table_reference_ 
4. SET _assignment_list_ 
	- _assignment_list_: 
		 _assignment_ [, _assignment_] ...
		- _assignment_: 
			_col_name_ = _value_ 
			- _value_: 
				{_expr_ | DEFAULT} 
1. [WHERE _where_condition_] 
2. [ORDER BY ...] 
3. [LIMIT _row_count_] 
