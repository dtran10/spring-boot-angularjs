FROM frolvlad/alpine-oraclejdk8:slim

VOLUME /tmp

EXPOSE 8080

ADD build/libs/demo-app-*.jar app.jar

RUN sh -c 'touch /app.jar'

ENV JAVA_OPTS=""

ENTRYPOINT ["sh", "-c", "java $JAVA_OPTS -jar /app.jar"]
