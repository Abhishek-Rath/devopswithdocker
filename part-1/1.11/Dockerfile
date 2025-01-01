FROM openjdk:8

# Set the working directory
WORKDIR /usr/src/myapp

# Copy all files into the container
COPY . .

# Ensure mvnw is executable
RUN chmod +x ./mvnw

# Run the Maven package command using mvnw
RUN ./mvnw package

# Expose port 8080
EXPOSE 8080

# Command to run the application
CMD ["java", "-jar", "./target/docker-example-1.1.3.jar"]
