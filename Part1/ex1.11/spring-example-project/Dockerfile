# Exercise 1.11: SPRING
# Submit the Dockerfile used to create a container to run
# the Java Spring project.

# Java 8 requirement
FROM openjdk:8

EXPOSE 8080

WORKDIR /usr/src/app

COPY . .

RUN ./mvnw package

CMD ["java", "-jar", "./target/docker-example-1.1.3.jar"]
