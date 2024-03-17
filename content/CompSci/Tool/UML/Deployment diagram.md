---
tags:
  - CompSci/tool/UML
---
# Deployment diagram
### Description:
- [[Deployment]]
- Model the physical architecture of a system
- Describes what existing systems will system need to interact or integrate with
- Show the relationships between the software and hardware components in the system and the physical distribution of the processing.
- Include:
	- Node:
		- Represent by a 3D box
	- Component:
		- Represent with 2D rectangle
	- Relationship between nodes:
		- Represent by line
### Draw
```plantuml
left to right direction
title SlideView deployment diagram
node "Windows (Desktop Computer)"{
	component "Desktop application( SlideView)" as d
}

node "ESCi server (x86)"{
	node "Virtual Machine (Linux)"{
		component "Backend server (Slideserve)" as b
	}
}

node "Server"{
	component "File server(Windows Sile Server)" as f
}

node "Server2" {
	component "Database(MySQL)" as d2
}
d --> b : "<TCP>"
b --> f : "SMB"
b --> d2 : "JDBC"
```
