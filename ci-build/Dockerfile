FROM maven:3.6-adoptopenjdk-11
COPY settings.xml /usr/share/maven/ref/
COPY helm /usr/local/bin/helm
COPY skaffold-linux-amd64 /
RUN <<EOR
    cd /
    apt-get update && sudo apt-get install -y apt-transport-https
    curl -s https://packages.cloud.google.com/apt/doc/apt-key.gpg | apt-key add -
    echo "deb https://apt.kubernetes.io/ kubernetes-xenial main" | tee -a /etc/apt/sources.list.d/kubernetes.list
    apt-get update
    apt-get install -y kubectl=1.16.2
    install skaffold /usr/local/bin/
EOR