FROM mysql:latest

RUN --mount=source=/docker-entrypoint-initdb.d  \
    mysql -u root -e 'CREATE DATABASE IF NOT EXISTS mydatabase;'

EXPOSE 3306

ENV MYSQL_ROOT_PASSWORD='mypass'  
CMD ["mysqld"]