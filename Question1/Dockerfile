FROM ubuntu
RUN apt-get update \
    && apt-get install nginx -y \
    && echo "daemon off;" >> /etc/nginx/nginx.conf
RUN mkdir -p /run/nginx
ADD index.html /usr/share/nginx/html/
ADD default /etc/nginx/sites-available/
EXPOSE 80
CMD ["nginx"]
