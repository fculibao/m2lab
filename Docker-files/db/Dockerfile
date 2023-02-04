FROM arm64v8/mysql:latest
LABEL Project="Vprofile"
LABEL Author="Ferdie"

# ENV MYSQL_ROOT_PASSWORD="vprodbpass" >>> should be equal to jdbc.password=vprodbpass on application.properties
ENV MYSQL_ROOT_PASSWORD="vprodbpass"   
ENV MYSQL_DATABASE="accounts"

# copy db back up script to the docker image ( db_backup.sql should be in this directory )
ADD db_backup.sql docker-entrypoint-initdb.d/db_backup.sql

CMD service mysql start

