---
mindmap-plugin: basic
tags:
  - CompSci/tool/UML
---
# Use case diagram
### Description:
- It is a model of the system's intended functionality (use cases) and its environment (actors). 
	- Define the user as a role
	- User can be another system
- Includes:
	- Use cases: 
		- Represents with a circle
		- Describe a [[Functional requirement|functional requirement]] that a system performs to achieve the user’s goal. 
		- A use case must yield an ==observable result== that is of value to the user of the system.
	- Actors: an icon for that actor
		- Represents with an icon for that actor
		- An actor represents a role of a user that interacts with the system that you are modeling. 
		- The user can be a human user, an organization, a machine, or another external system.
	- Subsystems: a folder
		- Represents with a folder
		- Subsystems are a type of stereotyped component that represent independent, behavioral units in a system. 
		- Subsystems are used in class, component, and use-case diagrams to represent large-scale components in the system that you are modeling.
	- Relationships in use-case diagrams: 
		- Represents with a simple arrow
		- A connection between model elements. 
		- A UML relationship is a type of model element that adds semantics to a model by defining the structure and behavior between the model elements.
### Draw
- 
  ```plantuml
	skinparam monochrome true
	left to right direction
	actor Guest as g
	package Professional {
	  actor Chef as c
	  actor "Food Critic" as fc
	}
	package Restaurant {
	  usecase "Eat Food" as UC1
	  usecase "Pay for Food" as UC2
	  usecase "Drink" as UC3
	  usecase "Review" as UC4
	}
	fc --> UC4
	g --> UC1
	g --> UC2
	g --> UC3
	```
- 