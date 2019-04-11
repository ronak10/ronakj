FROM openjdk
FROM ubuntu
RUN apt-get update && apt-get install -y maven
COPY pom.xml /usr/local/maven-demo/pom.xml
COPY src /usr/local/maven-demo/src
WORKDIR /usr/local/maven-demo
RUN mvn package
CMD ["java","-cp","target/maven-demo-1.0-SNAPSHOT.jar","com.ronak.App"] 
