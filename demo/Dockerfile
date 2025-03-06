# Base image olarak OpenJDK kullan
FROM openjdk:17-jdk-slim

# Uygulama JAR dosyasını container içine kopyala
ARG JAR_FILE=target/demo-0.0.1-SNAPSHOT.jar
COPY ${JAR_FILE} app.jar

# Container başladığında Spring Boot uygulamasını çalıştır
ENTRYPOINT ["java", "-jar", "/app.jar"]
