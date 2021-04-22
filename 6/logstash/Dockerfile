FROM ubuntu:18.04
LABEL maintainer="jkeauctions@gmail.com"
ENV REFRESHED_AT 2021-4-21

RUN apt-get -qq update
RUN apt-get -qq install wget gnupg2 openjdk-8-jdk
RUN wget -q0 - https://artifacts.elastic.co/GPG-KEY-elasticsearch | apt-key add
RUN echo "deb https://artifacts.elastic.co/packages/5.x/apt stable main" | tee -a /etc/apt/sources.list.d/elastic-5.x.list
RUN apt-get -qq update
RUN apt-get -qq install logstash
WORKDIR /usr/share/logstash
ADD logstash.conf /usr/share/logstash/
ENTRYPOINT [ "bin/logstash" ]
CMD [ "-f", "logstash.conf", "--config.relaod.automatic" ]
