FROM eclipse-temurin:18-jre-alpine

ADD . /usr/local/assets

WORKDIR /usr/local/assets

ENV profile=dev

COPY api/target ./

ENTRYPOINT java -jar -Dspring.profiles.active=$profile restful-booker-platform-assets-*.jar

