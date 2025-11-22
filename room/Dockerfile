FROM eclipse-temurin:18-jre-alpine

ADD . /usr/local/room

WORKDIR /usr/local/room

COPY target ./

ENV profile=dev
ENV authDomain=rbp-auth

ENTRYPOINT java -jar -Dspring.profiles.active=$profile target/restful-booker-platform-room-*.jar -D
