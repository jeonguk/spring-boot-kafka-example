# spring-boot-kafka-example
Spring boot web rest Kafka message producer consumer example

##
### Prerequisites
- JDK 1.8 or later
- Maven 3 or later (3.5)
- kafka

##
###
- kafka Install
  - Step 1: Download the code
```
https://www.apache.org/dyn/closer.cgi?path=/kafka/1.0.0/kafka_2.11-1.0.0.tgz
> tar -xzf kafka_2.11-1.0.0.tgz
> cd kafka_2.11-1.0.0
```
- Run
  - Step 2: Start the server
```
zookeeper start
> bin/zookeeper-server-start.sh config/zookeeper.properties
```
```
Kafka server start
> bin/kafka-server-start.sh config/server.properties
```

### More detail info 
  - https://kafka.apache.org/quickstart
  

## Application Quick Start

```
git clone https://github.com/jeonguk/spring-boot-kafka-example.git
cd spring-boot-kafka-example
```
```
mvn clean install
```
```
mvn boot:run
```


### Test
- Producer
  - http://localhost:8080/api/kafka/producer?data=Hello World

- Concumer
  - http://localhost:8080/api/kafka/consumer
