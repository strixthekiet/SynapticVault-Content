---
tags:
  - CompSci/network/protocol
aliases:
  - Hypertext Transfer Protocol (Secure)
---
# HTTP(s), Hypertext Transfer Protocol (Secure)
### Description:
- HTTP:
	- Send pure text
	- Port 80, 8008 or 8080
- HTTPS:
	- Encrypt and descript data
	- port 443 
	- use [[QUIC]] for
	- Use [[Transport Layer Security|TLS]] to encrypt data and hand-shaking
### Request includes:
- Request line:
	- Verb: Get, Post, Put, ..., 
	- Requested URI  
	- Protocol version
- Header variables 
	- Contain key value pairs.
	- Some of these are standard, such as user region which helps the receiver identify the requesting software agent.
	- Metadata about the message format or preferred message formats is also included here for HTTPS-based rest services.
	- Customizable
- The request body:
	- optional, only relevant to commands like post,put
	- data to be sent to the server and is only relevant for HTTP commands that send data
	- JSON or XML format
### Response includes:
- Response line:
	- HTTP version
	- [[#Response code]]
- Response header:
- Response body

### GET
- Retrieve data
### POST
- Create data
### PUT
- Create or alter data
### DELETE
- Delete data
### Response code:
- 200: success
- 400: client errors
- 500: server errors