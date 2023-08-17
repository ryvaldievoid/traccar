FROM openjdk:11-jre-slim

WORKDIR /src
COPY tracker-server.jar /src
COPY debug.xml .
COPY setup/* ./setup/
COPY schema/* ./schema/
COPY lib/* /src/lib/
ENV CLASSPATH=src/lib/*

EXPOSE 5055

CMD ["java", "-jar", "tracker-server.jar"]
