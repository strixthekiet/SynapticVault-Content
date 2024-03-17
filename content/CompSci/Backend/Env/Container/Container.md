---
tags:
  - CompSci/dev/backend/container
aliases:
  - container
---
# Container
### Description:
- A running user space around codes and its dependencies
- [[Machine Image]]
- Subject to [[Cold Start]]
- Make new [[Virtual machine|vm instance]] is boot whenever in use
	- Can be slow to boot
- Based on Linux technologies
	- Foundation of the Linux process.
		- Each Linux process has its own virtual memory address space, separate from all others, and Linux processes can be rapidly created and destroyed.
	- Linux namespaces.
		- Containers use Linux namespaces to control what an application can see, such as process ID numbers, directory trees, IP addresses, etc.
		- It’s important to note that Linux namespaces are not the same thing as Kubernetes namespaces, which you'll learn more about later in this course.
	- Linux cgroups.
		- Linux cgroups control what an application can use, such as its maximum consumption of CPU time, memory, I/O bandwidth, and other resources.
	- Union file systems :
		- to bundle everything needed into a neat package.
		- This requires combining applications and their dependencies into a set of clean, minimal layers.
### K8s container state:

| State      | Desc |
| ---------- | ---- |
| Waiting    |      |
| Running    |      |
| Terminated |      |
