FROM ubuntu:16.04
MAINTAINER vonzhou "vonzhou@163.com"
ENV REFRESHED_AT 2018-03-21
RUN apt-get -yqq update
RUN apt-get -yqq install ruby ruby-dev make nodejs
RUN gem install --no-rdoc --no-ri jekyll 

VOLUME /data
VOLUME /var/www/html
WORKDIR /data

ENTRYPOINT ["jekyll", "build", "--destination=/var/www/html"]
