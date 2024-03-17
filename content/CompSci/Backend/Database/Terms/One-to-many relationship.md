---
mindmap-plugin: basic
tags:
  - CompSci/database/ER-model
---
# One-to-many relationship
### Description:
- Relationship of one [[ER model entity instance|entity instance]]s to many [[ER model entity instance|entity instance]]s
	- Example: 1 customer can have many order
	- ```mermaid
	  %%{init: {'theme':'dark'}}%%
	  erDiagram
    CUSTOMER ||--o{ ORDER : places
    CUSTOMER {
        string name
        string custNumber
        string sector
    }
    ORDER {
        int orderNumber
        string deliveryAddress
    }
    ```
