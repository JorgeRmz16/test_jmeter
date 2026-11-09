FROM eclipse-temurin:17-jre

ENV JMETER_VERSION=5.6.3

RUN apt-get update && \
    apt-get install -y wget unzip && \
    wget https://archive.apache.org/dist/jmeter/binaries/apache-jmeter-${JMETER_VERSION}.tgz && \
    tar -xzf apache-jmeter-${JMETER_VERSION}.tgz && \
    mv apache-jmeter-${JMETER_VERSION} /opt/jmeter

ENV JMETER_HOME=/opt/jmeter
ENV PATH=$PATH:$JMETER_HOME/bin

WORKDIR /tests