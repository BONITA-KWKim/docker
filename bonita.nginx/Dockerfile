FROM centos:7

MAINTAINER kyugnwon.N.KIM (kyugnwon9010@gmail.com)

RUN yum update -y
RUN yum upgrade -y
#RUN touch /etc/yum.repos.d/nginx.repo
#RUN echo -e \ 
#"[nginx]\n\
#name=nginx repo\n\
#baseurl=http://nginx.org/packages/centos/7/$basearch/\n\
#gpgcheck=0\n\
#enabled=1" >> /etc/yum.repos.d/nginx.repo
RUN yum install epel-release -y
RUN yum install nginx -y
#RUN echo "\ndaemon off;" >> /etc/nginx/nginx.conf
#RUN chown -R www-data:www-data /var/lib/nginx

VOLUME ["/data", "/etc/nginx/site-enabled","/var/log/nginx"]

WORKDIR /etc/nginx

CMD ["nginx"]

EXPOSE 80
EXPOSE 443
