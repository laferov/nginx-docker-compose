FROM ubuntu:22.04
ADD index.html /start/
WORKDIR /start/ 
RUN apt-get -y update
RUN apt-get install -y nginx
RUN apt-get install -y vim 
RUN echo "daemon off;" >> /etc/nginx/nginx.conf
RUN cp index.html /var/www/html/index.html
RUN chmod 644 /var/www/html/index.html
CMD [ "nginx" ]
