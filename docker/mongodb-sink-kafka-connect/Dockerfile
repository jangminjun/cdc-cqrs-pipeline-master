FROM registry.redhat.io/amq-streams/kafka-34-rhel8:2.4.0-5

USER root:root
COPY ./mongo-plugins/ /opt/kafka/plugins/
USER 1001
