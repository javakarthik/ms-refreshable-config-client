# README #

Refreshable demo Config client accompanying source code for blog post at http://tech.asimio.net/2017/02/02/Refreshable-Configuration-using-Spring-Cloud-Config-Server-Spring-Cloud-Bus-RabbitMQ-and-Git.html

### Requirements ###

* Java 8
* Maven 3.3.x
* A [Config server](https://bitbucket.org/asimio/configserver) instance for this Demo Refreshable Config client to read remote properties from.

### Building the artifact ###

```
mvn clean package
```

### Running the application ###

```
java -Dspring.cloud.config.uri=http://localhost:8100 -jar target/demo-refreshable-config-client.jar
```
where a [Config server](https://bitbucket.org/asimio/configserver) instance is running at http://localhost:8100 in a *config-first* approach.

### Available endpoints ###

```
curl -v "http://localhost:8700/actors/1"
```

### Who do I talk to? ###

* ootero at asimio dot net
* https://www.linkedin.com/in/ootero