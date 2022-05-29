# SpringBootActuators
This microservice provides Actuator services
###### ![Latest version](https://img.shields.io/badge/Version-1.0-green.svg)

### Major dependencies and version
[![Java-11](https://img.shields.io/badge/OpenJDK-11-blue.svg)](https://openjdk.java.net/projects/jdk/11/)
![Spring boot-2.7.0](https://img.shields.io/badge/SpringBoot-2.7.0-blue.svg)
![Gradle-6.2](https://img.shields.io/badge/Gradle-6.2-blue.svg)

### Steps for deployment
1. **Generate JAR file**
   <br/> `./gradlew build`

2. **Build Docker image**
   <br/> `docker build -t actuator .`

3. **Run Docker image**
   <br/> `docker run -p 8092:8092 actuator`

## Documentation[]