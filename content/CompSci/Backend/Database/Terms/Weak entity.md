---
mindmap-plugin: basic
tags:
  - CompSci/database/ER-model
aliases:
  - weak entity
---

# Weak entity

## Description:
- Every row of that table cannot exist without depends on prior existence of another [[Strong entity|strong entity]]

## ID-dependent weak entity
- Has a composite identifier:
	- the first part of the identifier is [[Primary key|primary key]] for the [[Strong entity|strong entity]]
	- the second part of the identifier is [[Primary key|primary key]] for [[Weak entity|weak entity]] itself
	- Example: A book has many chapter

## Non-ID-dependent weak entity
- Doesn't include the [[Primary key|primary key]] of the parent's entity, it is instead foreign key
- It must have a relationship with the parent entity in order to be fully identified.