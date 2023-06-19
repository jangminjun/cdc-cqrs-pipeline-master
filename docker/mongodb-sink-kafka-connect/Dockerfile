FROM registry.redhat.io/amq-streams/kafka-34-rhel8:2.4.0-5

USER root:root
RUN yum install unzip -y
RUN mkdir -p /usr/share/java/

WORKDIR /

# kafka-connector-mongodb
ADD mongodb-kafka-connect-mongodb-1.10.1.zip /tmp/mongodb-kafka-connect-mongodb.zip
RUN unzip /tmp/mongodb-kafka-connect-mongodb.zip -d /opt/kafka/plugins/ \
&& rm /tmp/mongodb-kafka-connect-mongodb.zip
USER kafka:kafka
