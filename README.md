# Apache Kafka is an event streaming platform. 
## KAFKA Producer

To create a **KAFKA Producer**, you have to create a Java Class, lets say Producer.java . Then We need to define producer properties. 
Then create the producer and Create a producer record. Once they are ready, send the data
Follow the link below to read more about the properties of producer which one can set.
https://kafka.apache.org/documentation.

Three most important properties which are necessary are listed below.

**bootstrap.servers**: It is a list of the port pairs which are used for establishing an initial connection to the Kafka cluster. We use the bootstrap servers for making an initial connection to the cluster. This server is present in the host:port, host:port,... form.

**key.serializer**: It is a type of Serializer class of the key that is used to implement the org.apache.kafka.common.serialization.Serializer interface.

**value.serializer**: It is a type of Serializer class which implements the org.apache.kafka.common.serialization.Serializer interface.
Kafka consumer:
...................................................................................................

## KAFKA Consumer

To create a **KAFKA Consumer**, you have to create a Java Class, lets say ConsumerDemo.java. Then we need to define the consumer properties.
Then create a consumer,subscribe the consumer to a specific topic. Finally create a Poll loop to receive data.
Follow the link below to read more about the properties of consumer which one can set.
https://kafka.apache.org/documentation/#consumerconfigs
key.deserializer: It is a Deserializer class for the key, which is used to implement the org.apache.kafka.common.serialization.Deserializer interface.

These are some essential properties that are required to implement a consumer.

**value.deserializer**: A Deserializer class for value which implements the org.apache.kafka.common.serialization.Deserializer interface.

**bootstrap.servers**: It is a list of host and port pairs that are used to establish an initial connection with the Kafka cluster. It does not contain a full set of servers that a client requires. Only the servers which are required for bootstrapping are required.

**group.id**: It is a unique string that identifies the consumer of a consumer group.

**auto.offset.reset**: This property is required when no initial offset is present or if the current offset does not exist anymore on the server. There are the following values used to reset the offset values:

**earliest**: This offset variable automatically reset the value to its earliest offset.

**latest**: This offset variable reset the offset value to its latest offset.

**none**: If no previous offset is found for the previous group, it throws an exception to the consumer.

