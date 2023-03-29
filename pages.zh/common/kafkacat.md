# kafkacat 
## chatgpt 
kafkacat 是一款基于C语言编写的开源的Kafka命令行工具，可以用于生产和消费Kafka消息。它的主要功能包括：

1. 生产消息：可以使用命令行参数或文件读取方式生产消息。

2. 消费消息：可以消费指定的topic或者以正则表达式匹配topic。

3. 查看元数据：可以查看消费者组，分区信息，offset等。

除了上述主要功能外，kafkacat 还可以通过连接多个 broker 进行消息生产和消费，以及支持TLS/SSL 加密连接 Kafka。

下面是一些常见的 kafkacat 命令：

1. 生产消息：

```
kafkacat -b broker:port -t topic -P
```

2. 消费消息：

```
kafkacat -b broker:port -t topic -C
```

3. 消费指定分区的消息：

```
kafkacat -b broker:port -t topic -p partition -C
```

4. 查看分区信息：

```
kafkacat -L -b broker:port
```

5. 使用文件生产消息：

```
kafkacat -b broker:port -t topic -P -K: file.txt
```

6. 消费特定数量的消息：

```
kafkacat -b broker:port -t topic -C -c 10
```

7. 从指定 offset 开始消费消息：

```
kafkacat -b broker:port -t topic -C -o 123
```

总之，kafkacat 命令非常强大和灵活，适用于 Kafka 生产和消费中的各种场景。 

## tldr 
 
> 这是 `kcat` 命令的一个别名。

- 原命令的文档在：

`tldr kcat`
