---
tags:
  - CompSci/network/protocol
aliases:
  - OSI model
---
# Open Systems Interconnection, OSI Model
### Description:
- Conceptual framework used to describe the functions of a networking system.
- Characterizes computing functions into a universal set of rules and requirements in order to support interoperability between different products and software.
- Has 7 layers
- https://www.cloudflare.com/en-gb/learning/ddos/glossary/open-systems-interconnection-model-osi/
- The data must travel down the seven layers on the sending device and then travel up the seven layers on the receiving end.
### 7. Application layer:
- Sends and receive data from the app to the layer 6 with a chosen protocol
- [[HTTP(s)]]
### 6. Presentation:
- Compress the data and then it will hit the session layer
### 5. Session layer:
- Initiate the session
### 4. Transport layer:
- Segment the data
- [[Transmission Control Protocol]]
- [[UDP]]
### 3. Network layer: /internet layer?
- Broken the data down to packages
### 2. Data link layer:
- Break package down to frames
### 1. Physical layer:
- Sends frame as 0 and 1 in the cable