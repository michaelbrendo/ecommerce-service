# Ecommerce-service

## How to run
```bash
#Start zookeeper
bin/zookeeper-server-start.sh config/zookeeper.properties

#Start Kafka
bin/kafka-server-start.sh config/server.properties

#Run the project
./gradlew run

#Check if the topic was created
bin/kafka-topics.sh --list --bootstrap-server localhost:9092
~'ECOMMERCE_NEW_ORDER'

#Comsumer
bin/kafka-console-consumer.sh --bootstrap-server localhost:9092 --topic ECOMMERCE_NEW_ORDER --from-beginning

```
## Technology
- [Kafka](https://kafka.apache.org/)
  - [ZooKeeper](https://zookeeper.apache.org/)
- [Jabba/Java v11](https://github.com/shyiko/jabba)
