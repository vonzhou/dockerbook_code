FROM ubuntu:14.04
MAINTAINER vonzhou 
ENV REFRESHED_AT 2018-03-21

RUN apt-get -qq update
RUN apt-get -qq install nodejs npm
RUN ln -s /usr/bin/nodejs /usr/bin/node
RUN mkdir -p /var/log/nodeapp

ADD nodeapp /opt/nodeapp/

WORKDIR /opt/nodeapp
RUN npm install

VOLUME [ "/var/log/nodeapp" ]

EXPOSE 3000

ENTRYPOINT [ "nodejs", "server.js" ]

