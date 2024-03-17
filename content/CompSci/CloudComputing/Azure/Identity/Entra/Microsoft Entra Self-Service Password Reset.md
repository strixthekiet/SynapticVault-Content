---
tags:
  - CompSci/cloud-computing/Azure/service/EntraID
aliases:
  - Azure Entra SSPR
---
# Microsoft Entra Self-Service Password Reset
### Description:
- You can specify the minimum number of methods that the user must set up: one or two. 
	- For example, you might enable the mobile app code, email, office phone, and security questions methods and specify a minimum of two methods. 
	- Users can then choose the two methods they prefer, like mobile app code and email.
- If you're not signed in and you've forgotten your password or your password has expired, you can use SSPR in Microsoft Entra ID P1 or P2. 
	- It's also available with Microsoft 365 Apps for business or Microsoft 365.
- Requires atleast free trial plan
### Scope:
- **Disabled**: No users in the Microsoft Entra organization can use SSPR. This value is the default.
- **Enabled**: All users in the Microsoft Entra organization can use SSPR.
- **Selected**: Only the members of the specified security group can use SSPR. 
### Authenticate a password reset
- It's critical to verify a user's identity before you allow a password reset. Malicious users might exploit any weakness in the system to impersonate that user. Azure supports six different ways to authenticate reset requests.
- As an administrator, you can choose the methods to use when you configure SSPR. Enable two or more of these methods so that users can choose the ones they can easily use. The methods are:

|Authentication method|How to register|How to authenticate for a password reset|
|---|---|---|
|Mobile app notification|Install the Microsoft Authenticator app on your mobile device, then register it on the multifactor authentication setup page.|Azure sends a notification to the app, which you can either verify or deny.|
|Mobile app code|This method also uses the Authenticator app, and you install and register it in the same way.|Enter the code from the app.|
|Email|Provide an email address that's external to Azure and Microsoft 365.|Azure sends a code to the address, which you enter in the reset wizard.|
|Mobile phone|Provide a mobile phone number.|Azure sends a code to the phone in an SMS message, which you enter in the reset wizard. You can also choose to get an automated call.|
|Office phone|Provide a nonmobile phone number.|You receive an automated call to this number and press #.|
|Security questions|Select questions such as "In what city was your mother born?" and save their responses.|Answer the questions.|