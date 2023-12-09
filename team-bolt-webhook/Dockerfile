FROM maven:3.8-openjdk-8 AS build
COPY . . 
RUN mvn clean package -DskipTests

From openjdk:8
copy ==from=build /target/team-bolt-webhook-0.0.1-SNAPSHOT.jar team-bolt-webhook.jar
EXPOSE 8080
ENTRYPOINT ["java","-jar","team-bolt-webhook.jar"]