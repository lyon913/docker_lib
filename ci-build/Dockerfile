FROM maven:3.6-adoptopenjdk-11
COPY kubectl_1.16.6 /usr/local/bin/kubectl
COPY helm3_2_1 /usr/local/bin/helm
COPY skaffold-linux-amd64 /skaffold

RUN cd /
RUN install skaffold /usr/local/bin/