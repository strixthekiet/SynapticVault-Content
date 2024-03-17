---
tags:
  - CompSci/dev/software/architecture
---
# Pub-Sub
### Description:
- Uses [[RabbitMQ]]
- A `topic` is a shared string that allows applications to connect with one another through a common thread.
- Publishers push (or `publish`) a message to a Cloud Pub/Sub topic.
- Subscribers make a "`subscription`" to a topic where they will either pull messages from the subscription or configure webhooks for push subscriptions. Every subscriber must acknowledge each message within a configurable window of time.    
- To sum it up, a producer publishes messages to a topic and a consumer creates a subscription to a topic to receive messages from it.
- 
### Publisher:
### Subscriber:
- Subcription
### Topics:
- 