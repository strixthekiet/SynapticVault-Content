---
mindmap-plugin: basic
tags:
  - CompSci/database/SQL/clause
aliases:
  - HAVING
---
# SELECT
### Definition:
- `HAVING` is merged with [[WHERE clause optimization|WHERE]] if you do not use [[GROUP BY optimization]] or [[Aggregated functions|aggregated function]] functions (COUNT(), MIN(), and so on).
### SELECT
1. [ALL | DISTINCT | DISTINCTROW]


```sql
SELECT 
	[ALL | DISTINCT | DISTINCTROW ] 
	[HIGH_PRIORITY] [STRAIGHT_JOIN] 
	[SQL_SMALL_RESULT] [SQL_BIG_RESULT] [SQL_BUFFER_RESULT] 
	[SQL_NO_CACHE] [SQL_CALC_FOUND_ROWS] 
	_select_expr_ [, _select_expr_] ... 
	[_into_option_] 
	[FROM _table_references_ 
		[PARTITION _partition_list_]] 
	[WHERE _where_condition_] 
	[GROUP BY {_col_name_ | _expr_ | _position_}, ... [WITH ROLLUP]] 
	[HAVING _where_condition_] 
	[WINDOW _window_name_ AS (_window_spec_) 
		[, _window_name_ AS (_window_spec_)] ...] 
	[ORDER BY {_col_name_ | _expr_ | _position_} 
		[ASC | DESC], ... [WITH ROLLUP]] 
	[LIMIT {[_offset_,] _row_count_ | _row_count_ OFFSET _offset_}] 
	[_into_option_] [
	FOR {UPDATE | SHARE} 
		[OF _tbl_name_ [, _tbl_name_] ...] 
		[NOWAIT | SKIP LOCKED] 
	  | LOCK IN SHARE MODE] 
	[_into_option_] 
	
_into_option_: { 
	INTO OUTFILE '_file_name_' 
		[CHARACTER SET _charset_name_] 
		_export_options_ 
	  | INTO DUMPFILE '_file_name_' 
	  | INTO _var_name_ [, _var_name_] ... 
  }
```

