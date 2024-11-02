# Cloud-
Genai study jams
Pub/Sub is a messaging service for exchanging event data among applications and services.
A producer of data publishes messages to a Pub/Sub topic. A consumer creates a subscription to that topic. 
**A topic acts like a channel or a stream where messages are published. Producers send messages to a specific topic instead of directly to a consumer.


Subscribers either pull messages from a subscription or are configured as webhooks for push subscriptions. 
*1. Pull Subscription
How it Works: With a pull subscription, the subscriber explicitly requests (or "pulls") messages from the Pub/Sub server 
whenever it's ready to process them. This involves the subscriber making API calls periodically or on-demand to retrieve any new messages from the subscription.

Every subscriber must acknowledge each message within a configurable window of time.


What I  learnt
Set up a topic to hold data.
Subscribe to a topic to access the data.
Publish and then consume messages with a pull subscriber.
