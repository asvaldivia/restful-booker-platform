FROM eclipse-temurin:18-jre-alpine

ADD . /usr/local/message

WORKDIR /usr/local/message

COPY target ./

ENV authDomain=rbp-auth
ENV profile=dev

ENTRYPOINT java -jar -Dspring.profiles.active=$profile target/restful-booker-platform-message-*.jar -D
