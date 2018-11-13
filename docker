FROM openjdk:8-jdk-alpine
EXPOSE 9966
ARG PETCLINIC_JAR=target/spring-petclinic-1.5.2.war
ADD ${PETCLINIC_JAR} petclinic.war
ENTRYPOINT ["java","-Djava.security.egd=file:/dev/./urandom","-jar","/petclinic.war"]
