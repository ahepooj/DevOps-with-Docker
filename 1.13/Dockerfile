FROM openjdk:8-jdk-alpine
WORKDIR /app
RUN apk add maven
EXPOSE 8080
COPY . /app
# Following line was found to help with Windows OS, mvnw would fail
RUN mvn package
CMD ["java", "-jar", "./target/docker-example-1.1.3.jar"]
