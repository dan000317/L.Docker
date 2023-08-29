FROM ubuntu:latest
LABEL "Author"="Dan"
LABEL "Version"="1.0"
LABEL "Project"="Kool Form Pack"
ENV DEBIAN_FRONTEND=noninteractive
RUN apt update && apt install apache2 git -y
CMD ["/usr/sbin/apache2ctl", "-D", "FOREGROUND"]
EXPOSE 80
WORKDIR /var/www/html
VOLUME /var/log/apache2
ADD kool.tar.gz /var/www/html
COPY kool.tar.gz /var/www/html
