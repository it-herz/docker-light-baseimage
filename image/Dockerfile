FROM debian:jessie
MAINTAINER Bertrand Gouny <bertrand.gouny@osixia.net>

RUN echo "deb http://mirror.yandex.ru/debian/ sid main" >> /etc/apt/sources.list && apt update && apt dist-upgrade -y
ADD . /container
RUN /container/build.sh

ENTRYPOINT ["/container/tool/run"]
