## Build stage
#FROM maven:3.9.2-eclipse-temurin-17 AS build
#WORKDIR /app
## Copy the pom.xml
#COPY pom.xml .
## Copy the source code
#COPY user-service/src ./src
## Run Maven build
#RUN mvn clean package -DskipTests
#
## Run stage
#FROM openjdk:17-jdk-slim
#WORKDIR /app
#COPY --from=build /app/target/user-service-0.0.1-SNAPSHOT.jar app.jar
#EXPOSE 8081
#ENTRYPOINT ["java","-jar","app.jar"]