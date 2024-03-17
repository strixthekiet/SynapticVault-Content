---
tags:
  - CompSci/dev/Backend
---
# Backend
### Description:
- [[Recovery Point Objective]]
	- How long or much of data is ok to lose
- [[Recovery Time Objective]]
	- How long it takes for service to come back up running
- [[12 Factors App]]
### Bench-mark with ab:
- 
  ```bash
	sudo apt update
	sudo apt install apache2-utils -y
	ab -n 1000 -c 10 https://link.com
	```

### Types of deployment:
- Rolling update:
	- rolls out some nodes with new updates, one by one
- A/B:
	- Send updates to some nodes, to test the effectiveness
- Canary deployment:
	- Move to a certain group of user
- Blue/green deployment:
	- Both updates live together at the same time