# Use JDK 21 as base image
FROM eclipse-temurin:21-jre-jammy

# Set working directory
WORKDIR /app

# Copy the build artifact from Maven
ARG JAR_FILE=target/*.jar
COPY ${JAR_FILE} app.jar

# Expose the application port
EXPOSE 8080

# Run the application
ENTRYPOINT ["java", "-jar", "app.jar"]
