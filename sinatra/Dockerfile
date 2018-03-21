# failed
FROM ubuntu:14.04
MAINTAINER vonzhou "vonzhou@163.com"
ENV REFRESHED_AT 2018-03-21
RUN apt-get -yqq update && apt-get -yqq install curl gnupg build-essential
RUN gpg --keyserver hkp://keys.gnupg.net --recv-keys 409B6B1796C275462A1703113804BB82D39DC0E3
RUN curl -L get.rvm.io | bash -s stable
RUN source /usr/local/rvm/scripts/rvm
RUN rvm install 2.3.3
RUN gem install --no-rdoc --no-ri sinatra json redis

RUN mkdir -p /opt/webapp

EXPOSE 4567

CMD ["/opt/webapp/bin/webapp"]
