# Command Memo

- **ZooKeeper**
   - Path: `/Users/wuyichen/zookeeper-3.4.14/bin`
   - Commands
      - Start: `sh zkServer.sh start`
      - Stop: `sh zkServer.sh stop`
   - Port: 2181
- **Kafka**
   - Path: `/Users/wuyichen/kafka_2.11-2.2.0/bin`
   - Commands
      - Start: `sh kafka-server-start.sh ../config/server.properties`
      - Stop: Press Crtl+C
      - List all topics: `bash kafka-topics.sh --list --zookeeper localhost:2181`
      - Product a message to a topic: `bash kafka-console-producer.sh --broker-list localhost:9092 --topic <topic_name>`
      - Comsume a message from a topic: `bash kafka-console-consumer.sh --bootstrap-server localhost:9092 --topic <topic_name> --from-beginning`
   - Port: 9092
- **Kafka Connector Worker**
   - Path: `/Users/wuyichen/kafka_2.11-2.2.0/bin`
   - Commands
      - Start: `sh connect-distributed.sh ../config/connect-distributed.properties`
      - Stop: Press Crtl+C
   - Port: 8083
