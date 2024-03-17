---
tags:
  - CompSci/database
---
# Database design
### Description:
- Design a database
### Database design process:
1. Requirements analysis
	- Sources: user interviews, forms, reports,...
2. Component Design 
3. Implementation
### Workflow:
- For each [[Strong entity|strong entity]], create a table comprising its attributes and designate the primary key
- For each [[Weak entity|weak entity]], create a table comprising its attributes and including the primary key of its owning entity
	- absorb the attributes of the relationship
	- If relationship with the owning entity has any attributes, add them to this table
- For each [[One-to-one relationship]] between two entities, include the primary key of one entity as [[Foreign key]] in the table belonging to the other
- For each [[ER model relationship#Non-identifying relationship|non-identifying]] [[One-to-many relationship]] between two entities, include the primary key of the entity on the “1” side as a [[Foreign key]] in the table for the entity on the “N” side.
- For each [[Many-to-many relationship]] between two entities:
	- create a new table ([[ER model entity#Associative entity|Associative entity]] table) containing the[[Primary key|primary key]] of each entity as the [[Primary key|primary key]]
	- add any attributes of the relationship.

- ```mermaid
  erDiagram
  STUDENT ||--|| COURSES: OK
  STUDENT{
  	  string StudentID PK
  }
  ```



### [[Entity-relationship model]]