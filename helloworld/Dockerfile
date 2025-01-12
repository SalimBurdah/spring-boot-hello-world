FROM openjdk:17-jdk-alpine
VOLUME /tmp
COPY target/tech-test-0.0.1-SNAPSHOT.jar app.jar
ENTRYPOINT ["java","-jar","/app.jar"]