---
tags:
  - CompSci/cloud-computing/Azure/service/functionapp
---
# Azure Function App
### Description:
- [[FaaS]]
- Event-driven, serverless compute option that doesn’t require maintaining virtual machines or containers.
- With Azure Functions, an event wakes the function, alleviating the need to keep resources provisioned when there are no events.
- Functions can be either stateless or stateful. 
	- When they're stateless (the default), they behave as if they're restarted every time they respond to an event. 
	- When they're stateful (called Durable Functions), a context is passed through the function to track prior activity.
### two