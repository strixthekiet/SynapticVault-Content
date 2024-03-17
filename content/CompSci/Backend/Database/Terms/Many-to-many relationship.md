---
mindmap-plugin: basic
tags:
  - CompSci/database/ER-model
---
# Many-to-many relationship
### Description:
- Relationship of many [[ER model entity instance|entity instance]]s to many [[ER model entity instance|entity instance]]s
	- Example: many students can study many courses
	- ```mermaid
	  %%{init: {'theme':'dark'}}%%
	  erDiagram
	  STUDENT }|--o{ COURSE : studies
	  STUDENT {
	  string studentID
	  string studentName
	  string cohort
	  }
	  COURSE {
	  int courseID
	  string courseName
	  }
	  ```
