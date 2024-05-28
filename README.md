To create a **KAFKA Producer**, you have to create a Java Class, lets say Producer.java . Then We need to define producer properties. 
Then create the producer and Create a producer record. Once they are ready, send the data
Follow the link below to read more about the properties of producer which one can set.
https://kafka.apache.org/documentation.

Three most important properties which are necessary are listed below.

**bootstrap.servers**: It is a list of the port pairs which are used for establishing an initial connection to the Kafka cluster. We use the bootstrap servers for making an initial connection to the cluster. This server is present in the host:port, host:port,... form.

**key.serializer**: It is a type of Serializer class of the key that is used to implement the org.apache.kafka.common.serialization.Serializer interface.

**value.serializer**: It is a type of Serializer class which implements the org.apache.kafka.common.serialization.Serializer interface.
