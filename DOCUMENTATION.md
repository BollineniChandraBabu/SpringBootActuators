1. By using `Actuators` we can monitor and manage the application
* What is the health of the application?
* How many beans loaded into the application?
* What configuration properties loaded to the application?
* What is the heap info of the application?
* How many threads are running in the application?
* How many URL mappings are available in the application?

2. Add following dependency to enable actuators

* maven
```
<!-- https://mvnrepository.com/artifact/org.springframework.boot/spring-boot-starter-actuator -->
<dependency>
    <groupId>org.springframework.boot</groupId>
    <artifactId>spring-boot-starter-actuator</artifactId>
</dependency>

```
* Gradle
```
// https://mvnrepository.com/artifact/org.springframework.boot/spring-boot-starter-actuator
implementation group: 'org.springframework.boot', name: 'spring-boot-starter-actuator'
```

3. start the application and hit the following end point
``` 
http://localhost:9093/actuator/actuator 
```

4. By default, only `/health` endpoint is enabled in actuators.
```
http://localhost:9093/actuator/actuator/health 
```

5. To enable all the end points add the following line in the `application.properties` file
```
management.endpoints.web.exposure.include=*
```
then 13 end points will be exposed under actuators
![img.png](img.png)