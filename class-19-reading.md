# class 19 reading notes

## What are some use cases for both SNS and SQS?

both are important components for scalable, large scale, cloud-based  apps.

SNS is a distributed **publish-subscribe** service

SQS is a distributed **Queuing** service

## What is the difference betweeen SQS and SNS?

**SNS** (simple notification service) allows you to send "fast, flexible, fully managed push notification service that lets you send individual messages or to bulk messages to large numbers of recipients..."

These notifications are sent to subscribers as they are send by publishers to SNS.

you can send to various end points, even if you dont know the amount of subscriber... SNS is the way to go.

**SQS** (simple queuing service) is a "managed message queuing service that enables you to decouple and scale microservices, distributed systems, and serverless applications.

This is a queuing system.

"Messages are not pushed to receivers. Receivers have to poll SQS to receive messages. Messages can be stored in SQS for short duration of time (max 14 days)."

## Describe how to use SQS and SNS in a “fanout” pattern

**sns** publisher subscriber system

**sqs** queuing service for message process.

SNS's uses the fan out approach by way of one publishing a message to many subscribers (visual)(SQS, Lambda, Email)

SQS a system must poll the queue. messages in the queue are typically processed by a single user.

**SNS** *do other systems care about an event*

**SQS** *does your system care about an event*

## Explain how “push notifications” work, using SNS

The example is using to report a purchase. This is where we see a single purchase has  multiple services that are interested in knowing about that single event.From that single event we go from the transaction to the credit card service (authority service) after it gets validated we are able to publish an eveny about that topic(a analytics queue service, fraud service, or customer reminder service...) at the point of the customer reminder service we are able to send a push notification saying "that you for your service".

When we deliver to those various services and one of those services (the analytics) would be the SQS service, this would queue the info sent in to store the  basic info in a database to "balance the books".

## How might a large scale, distributed application make use of a Queue system like SQS? (I just took notes instead)

- Compute

- Database

- Messaging "glue that keeps the pieces together"

sent between software components.
Can be sent in JSON format. Software dev can deside the formate.
message payload can be sent along with message attributes (if you want). You can encrypt your payload and leave the message attributes left alone.

You can send a message to a queue and once you get confirmation that is in the queue the message is stored. You can process whatever needs to happen within the queued message and then to show it is done the message can go away. A queue is a buffer between producers and consumers.

At AWS they have SQS. is a highly scalable queuing system that can scale as your traffic grows. Even as the traffic grows this without greater latency. AWS recently created a FIFO queue, this process in the order they arrive however it is not as scalable. "ordered message processing".

This (message groups) is a really divide and conquer approach to queuing messages that belong to a specific group, Since we would be using the queuing system we couldnt really scale however with these message groups we could take care of different areas at once with this feature, This allows us to scale.

**Public/Subcribe messaging** This is where a publisher can send a specific message to every subscriber. In AWS we have SNS which allows us to attach a topic to multiple destinations. (HTTP, Lambda, SQS). Each message is stored with multiple copies. Both SQS and SNS are built per request.

**Message-streams** Ordered when a new message gets sent it gets attached to the end of the stream. When you send a message to a stream it persists. When it read back you open an iterater... They are able to stay in that stream as long as you want (or declare), you are able to iterate as you want. You are able analyze a sequence of items and go back and forth. Instead of having to independtly  process an item in a queue.

Long polling. Is giving you the heads up if there is info inside of the queue, instead of having this be a contstant wall of data, Long polling takes about 20 seconds for us to get that info every 20 seconds. This is a cheaper method.

## Things I want to know more about

streams

FIFO queues
