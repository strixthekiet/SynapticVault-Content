---
tags:
  - CompSci/database/SQL/aggregate-function
---
# [AVG([DISTINCT] _expr_) [_over_clause_]]
### Description:
- Returns the average value of ``_`expr`_``. The `DISTINCT` option can be used to return the average of the distinct values of _`expr`_.
- If there are no matching rows, [`AVG()`](https://dev.mysql.com/doc/refman/8.2/en/aggregate-functions.html#function_avg) returns `NULL`. The function also returns `NULL` if _`expr`_ is `NULL`.
- This function executes as a window function if _`over_clause`_ is present. _`over_clause`_ is as described in [Section 12.20.2, “Window Function Concepts and Syntax”](https://dev.mysql.com/doc/refman/8.2/en/window-functions-usage.html "12.20.2 Window Function Concepts and Syntax"); it cannot be used with `DISTINCT`.
- ```sql
    SELECT student_name, AVG(test_score)
           FROM student
           GROUP BY student_name;
           ```

