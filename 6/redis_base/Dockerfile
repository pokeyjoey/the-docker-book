FROM ubuntu:18.04
LABEL maintainer="jkeauctions@gmail.com"
ENV REFRESHED_AT 2021-4-21

RUN apt-get -yqq update
RUN apt-get install -yqq software-properties-common
RUN add-apt-repository ppa:chris-lea/redis-server
RUN apt-get -yqq update
RUN apt-get -yqq install redis-server redis-tools

VOLUME [ "/var/lib/redis", "/var/log/redis" ]

EXPOSE 6379
CMD []
