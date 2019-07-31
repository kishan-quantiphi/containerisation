FROM ubuntu:16.04

RUN apt-get update \
    && apt-get install -y nginx \
    && rm -rf /var/lib/apt/lists/* /tmp/* /var/tmp/* \
    && echo "daemon off;" >> /etc/nginx/nginx.conf


EXPOSE 80
CMD rm -rf /var/www/html/* && echo "<html><h1>$HOSTNAME</h1></html>" >> /var/www/html/index.html && service nginx start
