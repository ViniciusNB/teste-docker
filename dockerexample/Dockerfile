FROM openjdk:11-ea-11-jdk-slim
ARG JAR_FILE=target/*.jar
COPY ${JAR-FILE} app.jar
RUN bash -c 'touch /app.jar'
ENTRYPOINT ["java","-Djava.security.egd=file:/dev/./urandom","-jar","/app.jar"]