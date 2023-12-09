# Use the official OpenJDK base image
FROM openjdk:latest

# Set the working directory in the container
WORKDIR /team-bolt-webhook

# Copy the JAR file built by Gradle into the container
COPY build/libs/team-bolt-webhook-0.0.1-SNAPSHOT.jar team-bolt-webhook.jar

# Expose the port your application will run on
EXPOSE 8080

# Command to run the Spring Boot application
CMD ["java", "-jar", "app.jar"]