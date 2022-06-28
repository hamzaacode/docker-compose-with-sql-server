#FROM openjdk:11-jre-slim
##VOLUME /tmp
##ADD target/spring-boot-data-jpa-0.0.1-SNAPSHOT.jar app.jar
##ENTRYPOINT ["java","-jar","/app.jar"]


#Let me explain some points:

# -- FROM: install the image of the Maven – JDK version.
# -- WORKDIR: path of the working directory.
# -- COPY: copy all the files inside the project directory to the container.
# -- RUN: execute a command-line inside the container: mvn clean install to install the dependencies in pom.xml.
# -- CMD: run script mvn spring-boot:run after the image is built.

FROM openjdk:11-jre-slim
VOLUME /tmp
ADD target/spring-boot-data-jpa-0.0.1-SNAPSHOT.jar app.jar
ENTRYPOINT ["java","-jar","/app.jar"]