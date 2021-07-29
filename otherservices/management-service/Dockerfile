FROM openjdk:11
MAINTAINER phoenixcontact.com.cn
RUN mkdir /kogito
RUN mkdir /kogito/config
WORKDIR /kogito
ADD config/application.properties /kogito/config/application.properties
ADD management-console-1.8.0.Final-runner.jar /kogito/app.jar
ENTRYPOINT ["java","-jar","-Duser.timezone=Asia/Shanghai","/kogito/app.jar"]