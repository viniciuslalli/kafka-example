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
