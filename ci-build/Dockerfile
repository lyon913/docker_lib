FROM maven:3.6-adoptopenjdk-11

COPY settings.xml /usr/share/maven/ref/
COPY kubectl_1.16.6 /usr/local/bin/kubectl
COPY helm3.2.1 /usr/local/bin/helm
COPY skaffold-linux-amd64 /skaffold

RUN cd /
RUN install skaffold /usr/local/bin/