---
mindmap-plugin: basic
tags:
  - CompSci/dev/backend/vm
aliases:
  - vm instance
  - virtual machine
---
# Virtual machine
### Description:
- The virtualization or emulation of a computer system, usually Linux
- Based on computer architectures and provide the functionality of a physical computer.
- One or more virtual “guest” machines run on a physical “host” machine.  
### A system virtual machine(type 1):
- A fully virtualized to substitute for a physical machine. 
- A system platform supports the sharing of a host computer’s physical resources between multiple virtual machines, each running its own copy of the operating system. 
- This virtualization process relies on a [hypervisor](https://www.vmware.com/topics/glossary/content/hypervisor.html), which can run on bare hardware, such as [VMware ESXi](https://www.vmware.com/products/esxi-and-esx.html), or on top of an operating system.
### A process virtual machine(type 2):
- allows a single process to run as an application on a host machine, providing a platform-independent programming environment by masking the information of the underlying hardware or operating system. 
- An example of a process VM is the Java Virtual Machine, which enables any operating system to run Java applications as if they were native to that system.   

### Network of a VM:
- Each [[Virtual machine|vm instance]] has 2 IP address:
	- [[Private IP Address]]
		- When create a VM in Google Cloud, its symbolic name is registered with an internal [[Domain naming service|DNS]] service that translates the name to an internal IP address.
	- [[Public IP Address|External IP Address]]
		- Can allow connections from hosts outside of the project.
		- Optional
---