# Kafka_Hands_On-
Kafka Quickstart

## Installing Kafka

  - wget https://dlcdn.apache.org/kafka/3.8.0/kafka_2.13-3.8.0.tgz
  - $ tar -xzf kafka_2.13-3.8.0.tgz
  - $ cd kafka_2.13-3.8.0

## Starting Kafka Environment

  - $ bin/zookeeper-server-start.sh config/zookeeper.properties  # Start the ZooKeeper service
  - $ bin/kafka-server-start.sh config/server.properties         # Start the Kafka broker service

## Creating Topic

  - bin/kafka-topics.sh --create --topic kafka-implementation --bootstrap-server localhost:9092

## Display usage information

  - bin/kafka-topics.sh --describe --topic kafka-implementation --bootstrap-server localhost:9092

## Write into Topic

  - bin/kafka-console-producer.sh --topic kafka-implementation --bootstrap-server localhost:9092

## Reading from Topic

  - bin/kafka-console-consumer.sh --topic kafka-implementation --from-beginning --bootstrap-server localhost:9092

## Import/Export data as streams with Kafka connect

  - $ bin/connect-standalone.sh config/connect-standalone.properties config/connect-file-source.properties config/connect-file-sink.properties  #2 connectors and 3 configuration file

## 
