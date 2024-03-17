---
mindmap-plugin: basic
tags:
  - CompSci/database/SQL/statement/data-manipulation
aliases:
  - SELECT
  - Select
  - select
---

# SELECT statement

## Descriptions:
- used to retrieve rows selected from one or more tables, and can include [[UNION]] operations and subqueries.
- [[Intersect operation]] and [[EXCEPT]] operations are also supported.
- The [[Union operation|UNION]], [[Intersect operation|INTERSECTION]], and [[EXCEPT]] operators are described in more detail later in [[SQL Subqueries]]

## SELECT 

- \[ ALL | DISTINCT | DISTINCTROW ]
	- The ALL and DISTINCT modifiers specify whether duplicate rows should be returned.
	- ALL (the default) specifies that all matching rows should be returned, including duplicates.
	- DISTINCT (DISTINCTROW) specifies removal of duplicate rows from the result set.
	- DISTINCT can be used with a query that also uses WITH ROLLUP.
- select_expr \[, select_expr] ...
	- Each _select_expr_ indicates a column that you want to retrieve.
		- Can be `col1_name - col2_name AS new_name`
	- There must be at least one _`select_expr`_
	- * denotes select all _select_expr_
- \[ FROM ] `table_references`
	- `table_references` is returned from [[JOIN clause]]
		- Even if only used `TableA, TableB` or `TableA`
- \[ [[WHERE clause optimization|WHERE]] condition]
	- Indicates the condition or conditions that rows must satisfy to be selected.
	- In the WHERE expression, you can use any of the functions and operators that MySQL supports, except for [[Aggregated functions|aggregated function]]  (group).
		- See Section 9.5, “Expressions”, and Chapter 12, Functions and Operators.
	- Where col_name LIKE "XXX%";
- \[ [[GROUP BY optimization|GROUP BY]] {_col_name_ | _expr_ | _position_}, ... \[ WITH ROLLUP ]]
	- SELECT CITY, COUNT(*) AS NumberOfVendors FROM VENDORS GROUP BY City;
	- The Group By clause calculates the number of vendors in each city.
	- Using Group By we don’t need to specify each city. The statement will find all cities in the City column.
	- The Group By statement can contain multiple columns
	- The Group By statement can be nested (group inside group)
	- Most SQL implementations do not allow to group a column with variable length data type (we will cover data types later)
	- Group By clause come after any WHERE clause and before any ORDER BY clause
	- When using GROUP BY, instead of WHERE keyword, the HAVING  clause should be used.  
	- If we use the WHERE condition, it will be applied before grouping.
- \[ [[HAVING clause|HAVING]] _where_condition_]
- \[ [[ORDER BY optimization|ORDER BY]] {_col_name_ | _expr_ | _position_}
		\[ASC | DESC]
## SELECT ... INTO Statement
- 
## [[JOIN clause]]