# Spring Boot Kafka Reactive Project

## Description

This is a sample Spring Boot project that demonstrates the integration of Kafka with a Spring Reactive application

## Table of Contents (Optional)
 
- [Getting Started](#getting-started)
   - [Technology](#technology)
   - [Installation](#installation)
- [Usage](#usage)
- [Contributing](#contributing) 

## Getting Started 

Follow the instructions below to set up the project on your local machine for development and testing purposes.

### Technology

- Java 17 or later
- Apache Kafka (for running locally)
- Maven

### Installation

Clone this repository and navigate to the project folder:

Ensure that Kafka is installed and running locally. You can download Kafka from the [official Apache Kafka website](https://kafka.apache.org/).

Start a ZooKeeper server (required by Kafka):

```bash
bin/zookeeper-server-start.sh config/zookeeper.properties
```

Start a Kafka broker:
```bash
bin/kafka-server-start.sh config/server.properties
```

## Usage

![Kafka topics](img/kafka_demo_application.png)

To showcase the functionality of the application, I have developed two distinct projects:

1. **Producer Project:**
   The producer project leverages the **Spring Boot Reactive framework** to extract a data stream from [Wikimedia Recent Changes](https://stream.wikimedia.org/v2/stream/recentchange). This project is designed to efficiently read the streaming data and subsequently transmit the messages to a Kafka broker.

2. **Consumer Project:**
   The consumer project complements the aforementioned producer by retrieving messages from the Kafka topic. The retrieved messages are then persisted into a DynamoDB database. This dual-project configuration not only demonstrates the integration of Spring Boot Reactive with Kafka for real-time data processing but also showcases the seamless storage of this data in a DynamoDB database, emphasizing end-to-end functionality within the application.

## Contributing

Contributions are welcome! Please read our [CONTRIBUTING.md](CONTRIBUTING.md) for details on how to contribute to this project.

## License

This project is licensed under the [MIT License](LICENSE).

## Contact

Create: [ali-bouali]

Project Link: [apache-kafka-with-spring-boot](https://github.com/ali-bouali/apache-kafka-with-spring-boot-reactive)
 
