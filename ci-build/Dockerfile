FROM maven:3.6-adoptopenjdk-11

COPY kubectl_v1_18_8 /usr/local/bin/kubectl
COPY helm3 /helm

RUN cd /
RUN install helm /usr/local/bin
