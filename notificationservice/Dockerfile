# FROM openjdk:17-jdk-slim
# WORKDIR /app
# COPY target/*.jar app.jar

# EXPOSE 8084
# CMD ["java", "-jar", "notification-service.jar"]

FROM openjdk:17-jdk-slim
VOLUME /tmp
ARG JAR_FILE=target/*.jar
COPY ${JAR_FILE} app.jar
ENTRYPOINT ["java","-jar","/app.jar"]

