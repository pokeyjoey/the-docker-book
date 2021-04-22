FROM ubuntu:18.04
LABEL maintainer="jkeauctions@gmail.com"
ENV REFRESHED_AT 2021-04-20
RUN apt-get -yqq update; apt-get -yqq install redis-server redis-tools
EXPOSE 6379
ENTRYPOINT ["/usr/bin/redis-server"]
CMD []
