---
mindmap-plugin: basic
tags:
  - CompSci/database/ER-model
aliases:
  - Entity
  - entity
  - Entities
  - entities
---
# ER Entity

### Description:
- An entity is something that users want to track.
	- Examples include customers, purchases, products, etc.
- Entities of a given type are grouped into an entity class such as EMPLOYEE (a collection of all EMPLOYEE entities) which are shown in all caps.
- An [[ER model entity instance|entity instance]] of an entity class is the occurrence of a particular entity, such as CUSTOMER 12345.
### Attributes:
- Entities have attributes, which describe the entity’s characteristics.
	- Examples include EmployeeName, DateOfHire and JobSkillCode.
- Attributes are shown with the first letter of ==each word capitalized==.
- An attribute has a data type (character, numeric, date, currency, etc.)
### [[Strong entity]]

### [[Weak entity]]

### Associative entity:
- An associative entity (also called an association entity) is used whenever a pure N:M relationship cannot properly hold attributes that are describing aspects of the relationship between two entities.
- A new entity is then created to:
	- link the two original entities
	- hold the attributes
### Subtype entity
- A subtype entity is a special case of another entity called supertype.
- An attribute of the supertype indicates which of the subtypes is appropriate for a given instance and is called a discriminator.
- Subtypes can be exclusive or inclusive:
	- if exclusive, the supertype relates to at most one subtype
	- if inclusive, the supertype can relate to one or more subtypes
- The relationships that connect supertypes and subtypes are called IS- A relationship because a subtype is the same entity as the supertype.
- The identifier of a supertype and all of its subtypes is the same attribute