FROM ubuntu

ENV DEBIAN_FRONTEND noninteractive

RUN apt-get update && apt-get install -y \
    nano \
    apache2 \
    php

COPY index.php /var/www/html
COPY ./apache/000-default.conf /etc/apache2/sites-available/000-default.conf
CMD ["apachectl", "-D", "FOREGROUND"]
EXPOSE 80


