FROM eclipse-temurin:21-jdk 

WORKDIR /app

COPY target/*.jar app.jar

EXPOSE 8081

ENV DB_ENDPOINT=host.docker.internal
ENV DB_PORT=3306
ENV DB_NAME=Despacho
ENV DB_USERNAME=root
ENV DB_PASSWORD=root

ENTRYPOINT ["java", "-jar", "app.jar"]