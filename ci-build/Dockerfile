FROM maven:3.6-adoptopenjdk-11

COPY kubectl_1_16_6 /usr/local/bin/kubectl
COPY helm3_2_1 /helm
COPY skaffold-linux-amd64 /skaffold

RUN cd /
RUN install helm /usr/local/bin
RUN install skaffold /usr/local/bin/