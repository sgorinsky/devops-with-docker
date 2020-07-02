FROM openjdk:8

COPY . .
RUN cd spring-example-project && ./mvnw package 
CMD ["java", "-jar", "./spring-example-project/target/docker-example-1.1.3.jar"]
