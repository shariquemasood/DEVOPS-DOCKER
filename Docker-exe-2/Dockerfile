FROM ubuntu:latest
MAINTAINER Sharique Masood <sharique.masood@tothenew.com>
RUN apt-get update && apt-get upgrade -y
RUN apt-get install nginx -y
RUN apt-get install gettext-base -y

ENV web=website1

COPY my.tmpl /etc/nginx/conf.d/my.tmpl
ADD website1 /usr/share/nginx/html/website1
ADD website2 /usr/share/nginx/html/website2


CMD /bin/sh -c "envsubst < /etc/nginx/conf.d/my.tmpl > /etc/nginx/conf.d/default.conf && nginx -g 'daemon off;'"

