---
tags:
  - CompSci/cloud-computing/Azure/Compute/virtual_machine
---
# Azure Virtual Machine
### 1. Overview:
- [[IaaS]]
	- pwsh: Az.Compute, AzVM
	- cli: az vm
- You can specify a name with up to 15 characters on a Windows virtual machine and 64 characters on a Linux virtual machine.
- Shutdown in VM doesnt actually shutdown, must shutdown externally
- Belongs to a [[Azure Resource Group|resource group]]
- Can buy a RI (Reserved Instance) as commited usage
	- up to 72% price savings compared to pay-as-you-go pricing
	- flexible and can easily be exchanged or returned for an early termination fee.
	- atleast 1 year
- **Storage costs** are charged separately for the Azure Storage used by the virtual machine. 
	- The status of the virtual machine has no relation to the Azure Storage charges that are incurred. 
	- You're always charged for any Azure Storage used by the disks.
- Your disk image can be uploaded to [[Azure Storage what]] what?
### 2. Activity log:
### 3. Access Control:
### 4. Tags:
### 5. Diagnostics and:
# B. Connect:
### 1. Connect:
- ![](https://learn.microsoft.com/en-us/training/wwl-azure/configure-virtual-machines/media/bastion-connections-29c60c68.png)
### 2. Bastion:
- 
# C. Networking:
# D. Settings:
### 1. Disks:
- https://learn.microsoft.com/en-us/azure/virtual-machines/managed-disks-overview
- Have at least two disks: 
	- an operating system disk 
		- registered as a SATA
		- has label `C:`
	- a temporary disk. 
		- labeled as the `D:` drive by default.
		- On Windows virtual machines, the temporary disk is labeled as the `D:` drive by default. This drive is used for storing the **pagefile.sys** file.
		- On Linux virtual machines, the temporary disk is typically `/dev/sdb`. This disk is formatted and mounted to `/mnt` by the Azure Linux Agent.
		- **Don't store data on the temporary disk. This disk provides temporary storage for applications and processes and is intended to only store data like page or swap files.**
	- one or more optional data disks. 
		- A data disk is a managed disk that's attached to a virtual machine to store application data, or other data you need to keep. 
		- Data disks are registered as SCSI drives and are labeled with a letter you choose. 
		- The size of a virtual machine determines how many data disks you can attach and the type of storage you can use to host the data disks.
		- Azure Storage vs Managed Disk:
			- Managed disks are stored as virtual hard disks (VHDs).
				- stored as page blob
				- The available types of disks are Ultra Solid State Drives (SSD), Premium SSD, Standard SSD, and Standard Hard Disk Drives (HDD).
			- Azure Storage support standard and premium
- you can migrate existing virtual machine disks to Premium Storage.
# E. Availability + scale:
### 1. VM Size:
- https://learn.microsoft.com/en-us/azure/virtual-machines/sizes
### 2. Availability and scale:
- Availability zone:
- Scaling: [[Azure Virtual Machine Scale Set]]
- [[Azure Availability Set]]

