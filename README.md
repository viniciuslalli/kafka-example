# Kafka Spring Boot Example

## Introduction

This project is a simple demonstration of integrating Apache Kafka with a Spring Boot application. It includes basic configurations to set up a Kafka producer and consumer within a Spring context.

## Prerequisites

- JDK 1.8 or later
- Maven 3.2+
- An instance of Apache Kafka running on `localhost:9092` (default)
- Apache ZooKeeper running on `localhost:2181` (default)

## Installation

1. Clone the repository to your local machine.
2. Ensure Kafka and ZooKeeper services are up and running.
3. Navigate to the root directory of the project through the command line.

## Configuration

Configuration files can be found under `src/main/resources/`. The default configuration assumes Kafka and ZooKeeper are running on their default ports locally. Update the `application.properties` file if your setup differs.

## Running the Application

Execute the following command to start the application:

```shell
mvn spring-boot:run


## Starting Apache Kafka and ZooKeeper on Windows

Before running the Kafka application, you need to start ZooKeeper and Kafka server. Here's how to get them up and running on Windows:

1. Open a command prompt and navigate to your Kafka directory.

2. Start ZooKeeper: 
.\bin\windows\zookeeper-server-start.bat .\config\zookeeper.properties
Leave this command prompt open.

3. Open another command prompt and navigate to your Kafka directory.

4. Start the Kafka server:
.\bin\windows\kafka-server-start.bat .\config\server.properties

Leave this command prompt open as well.

Your Kafka broker should now be running and connected to ZooKeeper.

## Initializing a Kafka Topic and Consuming Messages

To consume messages from a Kafka topic on Windows, follow these steps:

1. Ensure that ZooKeeper and Kafka server are running.

2. Open a new command prompt and navigate to your Kafka directory.

3. Start consuming messages from the topic `lalliscode` using the Kafka console consumer:

.\bin\windows\kafka-console-consumer.bat --topic lalliscode --from-beginning --bootstrap-server localhost:9092

This command will consume messages from the beginning of the topic `lalliscode` and print them to the command prompt.

Remember, for the consumer to show messages, there must be messages produced to the `lalliscode` topic. You can use the Kafka console producer or your Spring Boot application to send messages to the topic.


