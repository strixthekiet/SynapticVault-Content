---
mindmap-plugin: basic
tags:
  - CompSci/database/SQL
---

# SQL Subqueries

## Description:
- The subqueries are processed starting from the innermost query and working outward
- Each subquery returns values to the upper-level query
- Subqueries can only process a single column

## Example:

-
  ```sql
  SELECT name, listed_price
  FROM paintings
  WHERE listed_price > (
  SELECT AVG(listed_price)
  FROM paintings
  );
  ```