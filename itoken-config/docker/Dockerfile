FROM openjdk:8-jre
MAINTAINER Jovan <jovanliu.it@gmail.com>

ENV APP_VERSION 1.0.0-SNAPSHOT

RUN mkdir /app
COPY itoken-config-$APP_VERSION.jar /app/app.jar

ENTRYPOINT ["java", "-Djava.security.egd=file:/dev/./urandom", "-jar", "/app/app.jar", "--spring.profiles.active=prod"]

EXPOSE 8888