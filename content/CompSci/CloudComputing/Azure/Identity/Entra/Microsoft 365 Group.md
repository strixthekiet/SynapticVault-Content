---
tags:
  - CompSci/cloud-computing/Azure/service/EntraID
---
# Microsoft 365 Group
### Description:
- Can be a single [[Azure Identity]]
- Group members have access to a shared mailbox, calendar, files, SharePoint site, and more.
- Use security groups to set permissions for all group members at the same time, rather than adding permissions to each member individually.
### Dynamic user:
- Use dynamic membership rules to automatically add and remove group members. 
- When member attributes change, Azure reviews the dynamic group rules for the directory. 
- If the member attributes meet the rule requirements, the member is added to the group. 
- If the member attributes no longer meet the rule requirements, the member is removed.
## Dynamic device:
- **Security groups only** 
- Apply dynamic group rules to automatically add and remove devices in security groups. 
- When device attributes change, Azure reviews the dynamic group rules for the directory. 
- If the device attributes meet the rule requirements, the device is added to the security group. 
- If the device attributes no longer meet the rule requirements, the device is removed.