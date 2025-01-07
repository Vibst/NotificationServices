# Use the official OpenJDK image as base image
FROM openjdk:17-jdk-slim

# Set the working directory
WORKDIR /app

# Copy the JAR file into the container
COPY target/*.jar notification-service.jar

# Expose the port your Spring Boot application will run on (e.g., 8084)
EXPOSE 8084

# Run the Spring Boot application
ENTRYPOINT ["java", "-jar", "/app/notification-service.jar"]
