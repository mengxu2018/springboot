# Start with a base image containing Java runtime
FROM openjdk:8-jdk-alpine

# Add Maintainer Info
LABEL maintainer="xuhang@gmail.com"

# Make port 8080 available to the world outside this container
EXPOSE 8080

RUN mkdir -p /var/www/app

# Add a volume pointing to /tmp, can docker inspect container_id to see the corresponding dir in host machine
VOLUME /tmp

WORKDIR /var/www/app

COPY spring-boot-crud.jar .

  # Run the jar file
ENTRYPOINT ["java","-jar","/var/www/app/spring-boot-crud.jar"]