FROM confluentinc/cp-kafka-connect:7.0.1

USER root
RUN yum install unzip -y
RUN mkdir -p /usr/share/java/

WORKDIR /

# kafka-connector-mongodb
ADD mongodb-kafka-connect-mongodb-1.10.1.zip /tmp/mongodb-kafka-connect-mongodb.zip
RUN unzip /tmp/mongodb-kafka-connect-mongodb.zip -d /usr/share/java/ \
&& rm /tmp/mongodb-kafka-connect-mongodb.zip
