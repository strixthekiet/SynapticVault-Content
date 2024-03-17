---
tags:
  - CompSci/tool/UML
---
# Component diagram
### Description:
- Show the structure of the software system, which describes the software components, their interfaces, and their dependencies. 
- You can use component diagrams to model software systems at a high level or to show components at a lower, package level.
- Includes:
	- Component:
		- Represent with 2D rectangle
		- With ports
	- Component instances
		- Model elements that represent actual entities in a system.
	- Packages
		- Packages group related model elements of all types, including other packages.
	- Artifacts
		- Model elements that represent the physical entities in a software system. 
		- Represent physical implementation units, such as executable files, libraries, software components, documents, and databases.
	- Interfaces
		- Represents with ball and socket notation
			- In which the implementation dependency from a classifier to the provided interface is displayed as a circle (ball) and the usage dependency from a classifier to the required interface is displayed as a half-circle (socket). 
			- This notation is also called the external view.
		- Interfaces are model elements that define sets of operations that other model elements, such as classes, or components must implement. 
		- An implementing model element realizes an interface by overriding each of the operations that the interface declares.
	- Relationships in component diagrams
		- Dependency:
			- Represent with dashed arrow
		- Relationship is a connection between model elements. 
		- A UML relationship is a type of model element that adds semantics to a model by defining the structure and behavior between model elements.
### Draw:
- ![](https://cdn-images.visual-paradigm.com/guide/uml/what-is-component-diagram/06-component-diagram-with-subsystem.png)