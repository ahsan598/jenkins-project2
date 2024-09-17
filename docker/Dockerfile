# Use an official OpenJDK runtime as a parent image
FROM openjdk:17-alpine

# Set the working directory inside the container
WORKDIR /usr/src/app

# Expose the application port
EXPOSE 8070

# Environment variable to specify the app home directory
ENV APP_HOME /usr/src/app

# Copy the JAR file into the container
COPY target/ekart-0.0.1-SNAPSHOT.jar $APP_HOME/app.jar

# Set the entry point to run the Java application
ENTRYPOINT exec java -jar app.jar