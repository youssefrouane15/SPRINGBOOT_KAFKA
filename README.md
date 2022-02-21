# SPRINGBOOT_KAFKA
A kafka demo with spring boot

to start the apache kafka server we need to perform the set of the following commands:

- Start Apache Zookeeper- C:\kafka_2.12-0.10.2.1>.\bin\windows\zookeeper-server-start.bat .\config\zookeeper.properties
- Start Apache Kafka- C:\kafka_2.12-0.10.2.1>.\bin\windows\kafka-server-start.bat .\config\server.properties
- Next start the Spring Boot Application by running it as a Java Application.
- Next Start the consumer listening to the demo_topic: 
- C:\kafka_2.12-0.10.2.1>.\bin\windows\kafka-console-consumer.bat --bootstrap-server localhost:9092 --topic demo_topic --from-beginning
- Finally hit the url as follows- http://localhost:8080/api/kafka/producer?message=test
- This will trigger the message to be sent to the demo_topic. We can see afterwards in the consumer started that the message is recieved.




