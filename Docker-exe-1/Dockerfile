FROM ubuntu:latest
MAINTAINER Sharique Masood <sharique.masood@tothenew.com>
RUN apt-get update && apt-get upgrade -y
RUN apt-get install nginx -y

COPY default.conf /etc/nginx/conf.d/default.conf
ADD website1 /usr/share/nginx/html/website1
CMD ["nginx", "-g", "daemon off;"]

