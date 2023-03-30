# kafkacat 
## chatgpt 
Kafkacat is a command line utility tool that can be used to produce and consume messages from Apache Kafka clusters. It is commonly used for testing and debugging purposes, as well as for creating scripts and building applications that interact with Kafka.

The kafkacat command can be used with a number of different arguments and options to perform various tasks, including:

1. Producing messages: The -P option can be used to produce messages to a Kafka topic. This option requires the broker list, topic name, and message text to be specified. For example, the following command will produce a message to the "test" topic with the text "hello world":

```
kafkacat -P -b broker1:9092,broker2:9092 -t test -p 0 -K: -m "hello world"
```

2. Consuming messages: The -C option can be used to consume messages from a Kafka topic. This option requires the broker list and topic name to be specified. For example, the following command will consume messages from the "test" topic:

```
kafkacat -C -b broker1:9092,broker2:9092 -t test
```

3. Reading messages from a specific offset: The -o option can be used to read messages from a specific offset. For example, to read messages starting from offset 100:

```
kafkacat -C -b broker1:9092,broker2:9092 -t test -o 100
```

4. Consuming messages from the beginning: The -e option can be used to start consuming messages from the beginning of the topic:

```
kafkacat -C -b broker1:9092,broker2:9092 -t test -e
```

5. Consuming messages from the end: The -Z option can be used to start consuming messages from the end of the topic:

```
kafkacat -C -b broker1:9092,broker2:9092 -t test -Z
```

6. Displaying message keys: The -K option can be used to display message keys along with the message values:

```
kafkacat -C -b broker1:9092,broker2:9092 -t test -K:
```

Overall, kafkacat is a versatile and powerful command line tool that can be used to perform a range of tasks related to Kafka message production and consumption. 

## tldr 
 
> This command is an alias of `kcat`.

- View documentation for the original command:

`tldr kcat`
