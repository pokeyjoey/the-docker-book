FROM ubuntu:18.04
LABEL maintainer="jkeauctions@gmail.com"
ENV REFRESHED_AT 2021-04-21

RUN apt-get -yqq update
RUN apt-get -yqq install wget

VOLUME [ "/var/lib/tomcat8/webapps/" ]
WORKDIR /var/lib/tomcat8/webapps/

ENTRYPOINT [ "wget" ]
CMD [ "-?" ]
