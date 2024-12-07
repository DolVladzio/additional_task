FROM openjdk:19-jdk-alpine3.16

WORKDIR /app

COPY . .

RUN chmod 755 ./mvnw
RUN mvn clean package -Dmaven.test.skip=true

EXPOSE 8080

CMD ["java", "-jar", "./target/simplecrud-0.0.1-SNAPSHOT.jar", "--server.port=8080"]
