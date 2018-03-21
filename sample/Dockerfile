FROM ubuntu:14.04
MAINTAINER vonzhou "vonzhou@163.com"
ENV REFRESHED_AT 2018-03-21
RUN apt-get -yqq update && apt-get -yqq install nginx
RUN mkdir -p /var/wwww/html/website
ADD nginx/global.conf /etc/nginx/conf.d/
ADD nginx/nginx.conf /etc/nginx/nginx.conf
EXPOSE 80
