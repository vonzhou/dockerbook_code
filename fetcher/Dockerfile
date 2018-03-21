FROM ubuntu:14.04
MAINTAINER vonzhou "vonzhou@163.com"
ENV REFRESHED_AT 2018-03-21
RUN apt-get -yqq update
RUN apt-get -yqq install wget

VOLUME ["/var/lib/tomcat7/webapps/"]
WORKDIR /var/lib/tomcat7/webapps/

ENTRYPOINT ["wget"]
CMD ["-?"]

