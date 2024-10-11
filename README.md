# kafka-admin

 - [Kafka](https://docs.confluent.io/kafka/overview.html)
 - [Kafka api](https://docs.confluent.io/kafka/kafka-apis.html)
 - [Kafka admin api](https://docs.confluent.io/kafka/kafka-apis.html#admin-api)
 - [Kafka admin Java api](https://kafka.apache.org/37/javadoc/org/apache/kafka/clients/admin/Admin.html)

## Few Admin Command

### Create Toipc

```sh 
 kafka-topics.sh --bootstrap-server=http://localhost:9092 --create --topic test 
 kafka-topics.sh --bootstrap-server=http://localhost:9092  --create --topic test-one 
 kafka-topics.sh --bootstrap-server=http://localhost:9092 --create --topic test-two 
```

### Produce Message

```sh
kafka-console-producer.sh --bootstrap-server=http://localhost:9092 --topic test
```

### Consume Messages

```sh
  kafka-console-consumer.sh --bootstrap-server=http://localhost:9092 --topic test --group test-group.one
  kafka-console-consumer.sh --bootstrap-server=http://localhost:9092 --topic test --group test-group.two
  kafka-console-consumer.sh --bootstrap-server=http://localhost:9092 --topic test --group test-group.three
```
