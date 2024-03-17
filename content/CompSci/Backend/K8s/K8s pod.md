---
tags:
  - CompSci/dev/backend/container/K8s/object
aliases:
  - pod
  - pods
---
# K8s pod
### Description:
- A wrap around one or a set of [[Container|container]]s
	- If many containers share the **same storages**, they can be the same pot
- Smallest unit in Kubernetes that you can create or deploy.
- [[Container]]s share network name space, IP, network ports
- [[Container]]s in a same port communicate through 127.0.0.1
### Pod's phase status:
| State            | Des                                                                              |
| ---------------- | -------------------------------------------------------------------------------- |
| Pending          | being scheduled or images being pulled from registry                             |
| Running:         | after successfull attached to a node                                             |
| Failed           | a container terminated with failture and wont be restarting                      |
| Succeeded        | all containers finished running successfully and they wont be restarting         |
| Unknown          | state cant be retrieved                                                          |
| CrashLoopBackOff | one of the containers in the pod exited unexpectedly even after it was restarted |

---