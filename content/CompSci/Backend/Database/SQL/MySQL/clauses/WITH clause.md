---
mindmap-plugin: basic
tags:
  - CompSci/database/SQL/clause
aliases:
  - WITH
---
# WITH clause
### Definition:
-  [[Common table expression]]
### WITH
- [RECURSIVE] 
- _cte_name_ 
	- _`cte_name`_ names a single common table expression and can be used as a table reference in the statement containing the [[WITH clause]]
- [(_col_name_ [, _col_name_] ...)] 
- AS (_subquery_) 
	- The _`subquery`_ part of `AS (_subquery_)` is called the “subquery of the CTE” and is what produces the CTE result set. 
	- The parentheses following `AS` are required.
- [, _cte_name_ [(_col_name_ [, _col_name_] ...)] AS (_subquery_)] ...
