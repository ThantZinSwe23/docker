FROM php:7.2-fpm
 
RUN apt-get update -y && apt-get install -y \
    nano \
    nginx

COPY ./nginx/nginx-site.conf /etc/nginx/sites-enabled/default
COPY index.php /var/www/html
COPY entrypoint.sh /etc/entrypoint.sh

EXPOSE 80 443

ENTRYPOINT ["sh","/etc/entrypoint.sh"]