FROM ubuntu
MAINTAINER Fredrik Valdmanis and Stein Inge Morisbak

RUN echo deb http://archive.ubuntu.com/ubuntu precise universe >> /etc/apt/sources.list
RUN apt-get update
RUN apt-get install -q -y openjdk-7-jre-headless
ADD http://mirrors.jenkins-ci.org/war/latest/jenkins.war /root/jenkins.war

EXPOSE 8080
ENTRYPOINT ["java", "-jar", "/root/jenkins.war"]
