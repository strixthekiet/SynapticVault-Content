---
mindmap-plugin: basic
tags:
  - CompSci/database/ER-model
---
# One-to-one relationship
### Description:
- Relationship of one [[ER model entity instance|entity instance]]s to exactly one [[ER model entity instance|entity instance]]s
	- Example: 1 order can have only 1 customer
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
