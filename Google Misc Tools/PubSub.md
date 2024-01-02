Is a Kafka like messaging service that allows for asynchronous messaging between applications. 

## Steps a message in pubsub goes through
### List of steps :
1. A publisher sends a message.
2. The message is written to storage.
3. Pub/Sub sends an acknowledgement to the publisher that it has received the message and guarantees its delivery to all attached subscriptions.
4. At the same time as writing the message to storage, Pub/Sub delivers it to subscribers.
5. Subscribers send an acknowledgement to Pub/Sub that they have processed the message.    
6. Once at least one subscriber for each subscription has acknowledged the message, Pub/Sub deletes the message from storage.
### Flow chart of steps :
![[PubSub Message Lifecycle.canvas]]

## Local Testing

Pub sub has a local emulator for testing purposes. All you do is install the correct package, run the emulator and set the correct env variables
## Resources:
https://cloud.google.com/pubsub/architecture#data_plane_-_the_life_of_a_message