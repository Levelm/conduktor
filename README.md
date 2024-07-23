# Playing with docker and conduktor
### To execute services
```
docker compose up -d
```
### To run kafka commands
```
docker run --network demo_bridge --interactive --tty --rm apache/kafka bash
/opt/kafka/bin/kafka-topics.sh --bootstrap-server kafkabroker:9092 --list
/opt/kafka/bin/kafka-topics.sh --bootstrap-server conduktor-gateway:6969 --list
```

### UIs
- Gateway: http://localhost:8888
- Console: http://localhost:8080