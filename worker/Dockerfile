FROM maven:3.5-jdk-8-alpine AS builder

COPY src /src

COPY pom.xml ./

COPY Dockerfile ./

RUN mvn -f ./pom.xml clean install

FROM openjdk:8-jre-alpine

WORKDIR /target

COPY --from=builder /target .

CMD ["java","-jar", "/target/worker-jar-with-dependencies.jar"]
