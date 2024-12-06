FROM openjdk:19-jdk-alpine3.16

WORKDIR /app

COPY . .

RUN chmod 755 ./mvnw
RUN ./mvnw clean package

EXPOSE 8080

CMD ["java", "-jar", "./target/*.jar", "--server.port=8080"]
