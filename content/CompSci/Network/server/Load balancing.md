---
tags:
  - CompSci/network/server
aliases:
  - Load balancer
  - load balancing
---
# Load balancing
### Description:
- Efficiently distributing incoming network traffic across a group of backend servers, also known as a server farm or server pool.
	- ![](https://www.nginx.com/wp-content/uploads/2014/07/what-is-load-balancing-diagram-NGINX.png)
	- 
### Load Balancing Algorithms
- **Round Robin** – Requests are distributed across the group of servers sequentially.
- **Least Connections** – A new request is sent to the server with the fewest current connections to clients. The relative computing capacity of each server is factored into determining which one has the least connections.
- **Least Time** – Sends requests to the server selected by a formula that combines the  
    fastest response time and fewest active connections. Exclusive to NGINX Plus.
- **Hash** – Distributes requests based on a key you define, such as the client IP address or  
    the request URL. NGINX Plus can optionally apply a consistent hash to minimize redistribution  
    of loads if the set of upstream servers changes.
- **IP Hash** – The IP address of the client is used to determine which server receives the request.
- **Random with Two Choices** – Picks two servers at random and sends the request to the  
    one that is selected by then applying the Least Connections algorithm (or for NGINX Plus  
    the Least Time algorithm, if so configured).