---
mindmap-plugin: basic
tags:
  - CompSci/database/ER-model
aliases:
  - Relationship
  - relationship
---
# ER model relationship

## Description:
- [[ER model entity|Entities]] can participate in relationships with other [[ER model entity|entities]].
	- For example: CUSTOMER buys ITEM

## Binary relationship:
- Degree 2 meaning 2 [[ER model entity instance|entity instance]]s are related in a relationship ^0fec4dc1-7c03-29c1
- [[Many-to-many relationship]]
- [[One-to-many relationship]]
- [[One-to-one relationship]]

## Ternary relationship:
- Degree 3 meaning 3 [[ER model entity instance|entity instance]]s are related in a relationship
	- Example: 2 parents to have 1 children

## Cardinality:
- Specifies the requirement of how many [[ER model entity instance|entity instance]] can be from or to in a relationship
	- Min-max cardinalities:
		- Example: a department can exist with minimum one employee
		- Typically min is 0 or 1
		- In [[Mermaid entity relationship diagram]],  use [[Mermaid entity relationship diagram#^b8e348| relationship syntax]]

## Recursive relationship
- It is possible for an entity to have a relationship to itself—this is called a
recursive relationship (also known as a unary relationship)

- 
  ```mermaid
  %%{init: {'theme':'dark'}}%%
  erDiagram
  CUSTOMER ||--o{ CUSTOMER: "refers to"
  CUSTOMER {
  string name
  string custNumber
  string sector
  }
  ```