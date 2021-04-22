FROM ubuntu:18.04
LABEL maintainer="jkeauctions@gmail.com"
ENV REFRESHED_AT 2021-04-21
RUN apt-get -yqq update
RUN apt-get -yqq install ruby ruby-dev build-essential nodejs
RUN gem install jekyll -v 2.5.3
VOLUME /data
VOLUME /var/www/html
WORKDIR /data
ENTRYPOINT [ "jekyll", "build", "--destination=/var/www/html" ]
