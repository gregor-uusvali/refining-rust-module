# Introduction

When creating an application, sometimes the application needs to read in events from other applications. For example, if an application is reading in from a news feed, it needs to listen to the news application to get events from the feed.

This can be a tricky problem to solve as applications may not want to maintain an API that updates so frequently. Getting data from an API can also be a large use of resources as the database needs to be maintained and the application will need to handle high traffic.

Database polling is an inefficient solution for real time updates. For software that needs to update its information in real time, it would be difficult to use a database.

An alternative way for multiple services to communicate is by using message queues.

## What is a Message Queue?

Let's say you are making an application for a shop which contains a list of new products in stock. This list needs to be updated so that customers can see what has been added immediately. The new application can read from the shop's existing stock application.

For this feature, the shop application can communicate with the stock software synchronously to keep the list updated. 

The stock application can implement a message queue. Messages can be added on to the queue for other applications to read from. These messages can be kept in the queue and read from at any time. This means the messages can be processed in real time.

### Topics, Producers and Consumers

A message queue is made up of 3 parts:

- Topic - this defines the event that the queue is for. Since an application can listen to multiple queues, a topic needs to be defined as an identifier.
- Producer - A producer publishes events/messages to a topic. This would be added to an application so that other applications can read from it. The producer puts messages into the queue.
- Consumer - A consumer reads from the message queue in the other service. This collects the data and completes the asynchronous communication.

An application can have a producer which is read by many consumers in many other applications.

### Apache Kafka

Apache Kafka is a popular implementation of a message queue system. It is used widely in the software industry. Kafka topics can be defined for pushing events on to a queue via Kafka producers.

## Further Reading

[Event Streaming with Kafka](https://kafka.apache.org/documentation/)

[Gently Down the Stream](https://www.gentlydownthe.stream/)
