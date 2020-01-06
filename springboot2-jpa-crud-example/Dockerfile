FROM tomcat:jdk8-openjdk
VOLUME /tmp
COPY ./target/springboot2-jpa-crud-example-0.0.1.war /usr/local/tomcat/webapps/user-service.war
RUN sh -c 'touch /usr/local/tomcat/webapps/user-service.war'
ENTRYPOINT [ "sh", "-c", "java -Dspring.profiles.active=docker -Djava.security.egd=file:/dev/./urandom -jar /usr/local/tomcat/webapps/user-service.war" ]
