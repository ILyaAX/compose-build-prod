FROM ubuntu:20.04
WORKDIR /opt/app
ENV TZ=Asia/Novosibirsk
RUN ln -snf /usr/share/zoneinfo/$TZ /etc/localtime && echo $TZ > /etc/timezone
RUN apt update && apt install git -y && apt install default-jdk -y && apt install maven -y 
RUN git clone https://github.com/boxfuse/boxfuse-sample-java-war-hello.git /tmp
RUN mvn clean package --file /tmp/pom.xml && cp /opt/target/hello-1.0.war /opt/app
