FROM openjdk:8-jdk-alpine
COPY ./target/service.jar /usr/Sample_service/
WORKDIR /usr/Sample_service
ENV SPRING_PROFILES_ACTIVE=dev
EXPOSE 8080
RUN sh -c 'touch service.jar'
ENTRYPOINT ["java","-jar","service.jar"]
