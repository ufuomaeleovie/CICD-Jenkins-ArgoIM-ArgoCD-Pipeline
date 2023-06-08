# You can change this base image to anything else
# But make sure to use the correct version of Java
FROM adoptopenjdk/openjdk11:alpine

# Simply the artifact path
ARG artifact=target/spring-boot-web.jar
ADD target/spring-boot-starter-parent-2.2.4.RELEASE.jar spring-boot-starter-parent-2.2.4.RELEASE.jar

WORKDIR /opt/app

COPY ${artifact} app.jar

# This should not be changed
ENTRYPOINT ["java","-jar","app.jar"]
