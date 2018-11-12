FROM centos:7

MAINTAINER kyugnwon.N.KIM <noberto.kyungwon@gmail.com>

RUN yum update -y && yum upgrade -y

#setting nginx
RUN yum install epel-release -y
RUN yum install nginx -y
RUN echo "daemon off;" >> /etc/nginx/nginx.conf
#RUN chown -R www-data:www-data /var/lib/nginx

#VOLUME ["/data", "/etc/nginx/site-enabled","/var/log/nginx"]

WORKDIR /etc/nginx

CMD ["nginx"]

EXPOSE 80
EXPOSE 443
