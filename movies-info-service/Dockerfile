# Use a base image with Java and a compatible version of Linux (you can adjust the version as needed)
FROM adoptopenjdk:11-jre-hotspot

# Set the working directory inside the container
WORKDIR /app

# Copy the JAR file built from your Spring WebFlux application into the container
COPY build/libs/movies-info-service-0.0.1-SNAPSHOT.jar app.jar

# Expose the port that your Spring WebFlux application listens on
EXPOSE 8080

# Set the "local" profile as an environment variable
ENV SPRING_PROFILES_ACTIVE=local

# Command to run your Spring WebFlux application when the container starts
CMD ["java", "-jar", "app.jar"]
