FROM ubuntu

RUN apt-get update -y && apt-get install -y \
    nano \
    mysql-server 

EXPOSE 3306

CMD ["mysqld","--user","mysql"]