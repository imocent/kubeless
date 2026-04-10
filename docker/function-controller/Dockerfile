FROM bitnami/minideb:jessie

RUN echo "deb http://archive.debian.org/debian/ jessie main" > /etc/apt/sources.list \
    && echo "deb http://archive.debian.org/debian-security jessie/updates main" >> /etc/apt/sources.list

RUN install_packages ca-certificates

ADD kubeless-function-controller /kubeless-function-controller

ENTRYPOINT ["/kubeless-function-controller"]
