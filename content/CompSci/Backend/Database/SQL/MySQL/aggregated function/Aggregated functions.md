---
tags:
  - CompSci/database/SQL/aggregate-function
aliases:
  - aggregated function
---
# Aggregated functions
### Descriptions:
- https://dev.mysql.com/doc/refman/8.0/en/aggregate-functions.html#function_count
### Aggregate functions:
- [[AVG()]]
- [[BIT_AND()]]
- [[Bit_OR()]]
- [[BIT_XOR()]]
- [[COUNT()]] and [[COUNT#COUNT(DISTINCT)]]
- [[GROUP_CONCAT()]]
- 
- 
- [[MAX()]]
- [[MIN()]]
- [[STD()]]
- 
- |[`BIT_OR()`](https://dev.mysql.com/doc/refman/8.0/en/aggregate-functions.html#function_bit-or)|Return bitwise OR|
|[`BIT_XOR()`](https://dev.mysql.com/doc/refman/8.0/en/aggregate-functions.html#function_bit-xor)|Return bitwise XOR|
|[`COUNT()`](https://dev.mysql.com/doc/refman/8.0/en/aggregate-functions.html#function_count)|Return a count of the number of rows returned|
|[`COUNT(DISTINCT)`](https://dev.mysql.com/doc/refman/8.0/en/aggregate-functions.html#function_count-distinct)|Return the count of a number of different values|
|[`GROUP_CONCAT()`](https://dev.mysql.com/doc/refman/8.0/en/aggregate-functions.html#function_group-concat)|Return a concatenated string|
|[`JSON_ARRAYAGG()`](https://dev.mysql.com/doc/refman/8.0/en/aggregate-functions.html#function_json-arrayagg)|Return result set as a single JSON array|
|[`JSON_OBJECTAGG()`](https://dev.mysql.com/doc/refman/8.0/en/aggregate-functions.html#function_json-objectagg)|Return result set as a single JSON object|
|[`MAX()`](https://dev.mysql.com/doc/refman/8.0/en/aggregate-functions.html#function_max)|Return the maximum value|
|[`MIN()`](https://dev.mysql.com/doc/refman/8.0/en/aggregate-functions.html#function_min)|Return the minimum value|
|[`STD()`](https://dev.mysql.com/doc/refman/8.0/en/aggregate-functions.html#function_std)|Return the population standard deviation|
|[`STDDEV()`](https://dev.mysql.com/doc/refman/8.0/en/aggregate-functions.html#function_stddev)|Return the population standard deviation|
|[`STDDEV_POP()`](https://dev.mysql.com/doc/refman/8.0/en/aggregate-functions.html#function_stddev-pop)|Return the population standard deviation|
|[`STDDEV_SAMP()`](https://dev.mysql.com/doc/refman/8.0/en/aggregate-functions.html#function_stddev-samp)|Return the sample standard deviation|
|[`SUM()`](https://dev.mysql.com/doc/refman/8.0/en/aggregate-functions.html#function_sum)|Return the sum|
|[`VAR_POP()`](https://dev.mysql.com/doc/refman/8.0/en/aggregate-functions.html#function_var-pop)|Return the population standard variance|
|[`VAR_SAMP()`](https://dev.mysql.com/doc/refman/8.0/en/aggregate-functions.html#function_var-samp)|Return the sample variance|
|[`VARIANCE()`](https://dev.mysql.com/doc/refman/8.0/en/aggregate-functions.html#function_variance)|Return the population standard variance|
### [[GROUP BY optimization|GROUP BY]] modifier:
### MySQL handling of [[GROUP BY optimization|GROUP BY]]:
### Detection of functional dependence:
